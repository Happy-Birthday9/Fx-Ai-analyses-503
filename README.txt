TRADING STRATEGY VAULT — TWELVE DATA ONLY

This build removes OpenAI, Gemini, and Groq completely.
Only Twelve Data is used for market data and technical signal generation.

Setup:
1. Open ai-config.js.
2. Put your Twelve Data API key in TWELVE_DATA_API_KEY.
3. Upload the files to your GitHub Pages/Netlify site.
4. Upload a Quotex chart screenshot.
5. The browser OCR reads the visible market/pair, then Twelve Data symbol search finds the instrument.
6. Twelve Data OHLC data is analyzed with EMA9, EMA21, RSI14 and candle direction.

Important:
- Twelve Data is a market-data/technical-analysis API, not a vision AI model.
- Screenshot market detection uses local browser OCR (Tesseract.js), not another AI API.
- Quotex OTC symbols may not exist in Twelve Data; if so, the app will show a symbol/data error rather than inventing a signal.
- Frontend API keys are visible to visitors. A backend is recommended for real secret protection.
