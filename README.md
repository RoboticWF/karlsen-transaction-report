# Karlsen Transaction Report

Generates a CSV file for all your Karlsen transactions.

Currently in alpha - no expected SLA.

## Want to just get to generating your report?

You can use the deployment at https://Karlsen-transaction-report.vercel.app/

## Requirement

- NodeJS (v16+)

## Usage

1. Download this repository and unzip (or clone it if you know how)
2. Open a terminal/cmd and go to the directory you downloaded this at, then run `npm install`. This will install dependencies.
3. Create a file `addresses.txt` in this directory. In this file, you will list all your address - one per line
```
Karlsen:myaddress
Karlsen:myotheraddress
Karlsen:anotherone
```
4. To generate your transaction report run `npm run generate`

This will generate the file `Karlsen-transactions.csv`. This CSV is currently compatible with Koinly only.

## Notes
- Compound transactions and transactions sending to yourself are ignored
- Assumes addresses from exchanges are treated as not your own
- If you notice the report is inaccurate, first make sure you actually listed all addresses you care about in `addresses.txt`

## Found this useful?

Consider donating to `Karlsen:qq6xkkf2t209dmlhmffshdagnkkhzufc5xdt03c3psgxv5yk7panqzwdm0pwp`
