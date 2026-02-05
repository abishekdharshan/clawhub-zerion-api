# Zerion API

Query crypto wallet portfolios, transactions, DeFi positions, and token prices across EVM chains and Solana using Zerion's MCP server.

## Overview

Access Zerion's interpreted crypto wallet data through MCP tools. Supports **EVM chains** (Ethereum, Polygon, Arbitrum, Optimism, Base, BSC, 50+ more) and **Solana**.

**Note**: API key required - get yours at https://developers.zerion.io

## Available Data

| Data Type | Description |
|-----------|-------------|
| Portfolio | Total wallet value, breakdown by chain |
| Transactions | Full transaction history with parsed actions |
| PnL | Profit/loss calculations |
| Positions | DeFi positions, staking, lending |
| Token Prices | Real-time pricing and historical charts |
| NFTs | Collections and individual NFT data |
| Gas Prices | Current gas prices across chains |

## Common Queries

### Portfolio Analysis
```
Get the portfolio for wallet 0x1234...
Show total value and breakdown by chain for 0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045
```

### Transaction History
```
Show recent transactions for 0x1234...
Get transaction history for 0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045 in the last 30 days
```

### DeFi Positions
```
Show all DeFi positions for 0x1234...
What protocols is 0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045 using?
```

### Token Analysis
```
Get current price of ETH
Show price chart for USDC over the last 7 days
Compare ETH price to SOL
```

### NFT Data
```
Show NFT collections owned by 0x1234...
Get details for Bored Ape #1234
List all NFTs in wallet 0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045
```

### Gas Prices
```
What are current gas prices on Ethereum?
Compare gas prices across all EVM chains
Show Solana transaction fees
```

## Tips

1. **Address Format**: Use 0x addresses only (e.g., 0xd8dA6BF26964aF9D7eEd9e03E53415D37aA96045)
2. **Multi-Chain**: Supports EVM chains and Solana
3. **Real-Time**: All data is real-time from Zerion's indexed data
4. **Auth Required**: API key needed - configure in MCP settings

## MCP Server Details

**URL**: `https://developers.zerion.io/mcp`
**Type**: Remote HTTP MCP server
**Auth**: API key required (get at https://developers.zerion.io)
**Docs**: https://developers.zerion.io/reference/building-with-ai

## Setup

1. Get your API key at https://developers.zerion.io
2. Add to your MCP configuration:

```json
{
  "zerion": {
    "url": "https://developers.zerion.io/mcp",
    "headers": {
      "Authorization": "Bearer YOUR_API_KEY"
    }
  }
}
```

## Related Resources

- API Docs: https://developers.zerion.io
- Zerion Dashboard: https://dashboard.zerion.io
- llms.txt: https://developers.zerion.io/llms.txt

## When to Use

Use this skill when researching wallet addresses, analyzing DeFi positions, getting real-time token prices, investigating transaction patterns, exploring NFT holdings, checking gas prices across chains, or validating customer/competitor data.
