# TariffTrust extension for Gemini CLI

US import duties and fees for an HTS code, an origin and a value, each with its official source, as tools of [Gemini CLI](https://github.com/google-gemini/gemini-cli): estimate one product, a whole import declaration or a batch, follow a product over the changes of the tariff, search the HTS, list the trade agreements and the questions an estimate may ask, read your saved estimates.

## Install

```bash
gemini extensions install https://github.com/tarifftrust/gemini-cli-extension
```

Gemini CLI asks for your TariffTrust API key, created on the API access page of your workspace (<https://tarifftrust.com/keys/>), and keeps it in your system keychain. The MCP server and the API are included in the plans with API access.

Then ask, for instance: “What US duty applies to 10,000 USD of men's cotton T-shirts from China?”

## Without the extension

The extension connects Gemini CLI to the TariffTrust MCP server, `https://api.tarifftrust.com/mcp/`, with your key as a Bearer token. Claude, Cursor, VS Code and the OpenAI and Claude APIs connect to it the same way: see <https://tarifftrust.com/api/mcp/>.

TariffTrust never classifies products, and an estimate is informational, not a customs determination.

## License

MIT
