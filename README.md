# Solana NFT Drop Project (adapted from Buildspace)

### Welcome 👋

To get started with this project, clone this repo and follow these commands:

1. cd into the `app` folder
2. Run `npm install` at the root of your directory
3. Run `npm run start` to start the project
4. Start coding!

Useful Command :
1. Candy Machine CLI v2 (deprecated)
`ts-node ~/Develop/_toolkit_/deprecated-clis/src/candy-machine-v2-cli.ts --version`

2. Upload NFT to Devnet
`ts-node ~/Develop/_toolkit_/deprecated-clis/src/candy-machine-v2-cli.ts upload -e devnet -k /Users/jonathankristanto/.config/solana/id.json -cp config.json ./assets/`

3. Verifying Upload

## Update 21-01-2024 
=================
The course tool is already outdated, so I'm using Sugar for Candy Machine V3, the newest tool from Metaplex

### Docs : 
- https://developers.metaplex.com/candy-machine/sugar
- https://docs.metaplex.com/developer-tools/sugar/guides/sugar-for-cmv3

### Repo : 
https://github.com/metaplex-foundation/sugar


Log 
====
jonathankristanto@Julias-MacBook-Air nft-drop-starter-project % sugar launch
Starting Sugar launch... 🚀 

>>> sugar validate

[1/1] 🗂  Loading assets
⠁ 
⚠️  missing `properties.category` for nft Vestimon, defaulting to image
⚠️  missing `properties.category` for nft JK First NFT, defaulting to image
⚠️  missing `properties.category` for nft JK-Collection, defaulting to image
▪▪▪▪▪ Validating 4 metadata file(s)...

Validation complete, your metadata file(s) look good.

>>> sugar upload

[1/4] 🗂  Loading assets
Found 4 asset pair(s), uploading files:
+--------------------+
| images    |      1 |
| metadata  |      1 |
+--------------------+

[2/4] 🖥  Initializing upload
▪▪▪▪▪ Connected
Funding address:
  -> pubkey: GwKWeDXLkBATWCJvbjtjrJE153tfHPmHgVEyKQTMZK55
  -> lamports: 81911 (◎ 0.000081911)
Signature: YePB5k4xxv3vwSpW5S6NSe2izJknJNj1gvDtzuaf3mxKsPBwbXnvuNrgD4YxCzVRDN4GtNRj5Me3UL8Uj1sND9b

[3/4] 📤 Uploading image files 

Sending data: (Ctrl+C to abort)
[00:00:05] Upload successful ███████████████████████████████████████████████████████████████████████████████████████████████████████████ 1/1

[4/4] 📤 Uploading metadata files 

Sending data: (Ctrl+C to abort)
[00:00:00] Upload successful ███████████████████████████████████████████████████████████████████████████████████████████████████████████ 1/1

4/4 asset pair(s) uploaded.

>>> sugar deploy


[1/3] 📦 Creating collection NFT for candy machine
Collection mint ID: ByaT3QaKCoejBfx3P416TN6K6mHBnfgNp1WfK8XjZUQc

[2/3] 🍬 Creating candy machine
Candy machine ID: CFor2AovWU2geVwLV8dVM1GHcrJBeTQXJDfs1EuNiMHz

[3/3] 📝 Writing config lines
Sending config line(s) in 1 transaction(s): (Ctrl+C to abort)
[00:00:01] Write config lines successful ███████████████████████████████████████████████████████████████████████████████████████████████ 1/1

>>> sugar verify

[1/2] 🍬 Loading candy machine
▪▪▪▪▪ Completed

[2/2] 📝 Verification
Verifying 3 config line(s): (Ctrl+C to abort)
[00:00:01] Config line verification successful █████████████████████████████████████████████████████████████████████████████████████████ 3/3

Verification successful. You're good to go!

See your candy machine at:
  -> https://www.solaneyes.com/address/CFor2AovWU2geVwLV8dVM1GHcrJBeTQXJDfs1EuNiMHz?cluster=devnet

✅ Command successful.