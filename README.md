# PIROCKET Root Domain GitHub Pages Setup

Stellar wallets check the root of your home domain to find the `stellar.toml` file:
`https://successclub.github.io/.well-known/stellar.toml`

Follow the instructions below to create your root domain site and upload the required TOML file:

## 🚀 deployment steps

1. **Create the GitHub Repository:**
   - Go to: https://github.com/new
   - Repository Name: **`successclub.github.io`** (Must be exactly this name!)
   - Public/Private: **Public**
   - Click **Create repository**

2. **Initialize Local Git and Deploy:**
   Open PowerShell in this folder (`c:\Users\money\pirocket-stellar\root-domain-setup`) and run the following commands:

   ```bash
   # Initialize git repository
   git init

   # Add all files (.nojekyll and .well-known/stellar.toml)
   git add -A

   # Commit the files
   git commit -m "feat: add stellar.toml for pirocket"

   # Set active branch name to main
   git branch -M main

   # Add your github remote
   git remote add origin https://github.com/successclub/successclub.github.io.git

   # Push changes
   git push -u origin main
   ```

3. **Verify:**
   - Check if `https://successclub.github.io/.well-known/stellar.toml` is working in your browser.
   - Once it responds with the TOML content, Stellar wallets will immediately recognize the PIROCKET logo without errors.
