# Gold Analytics V9 — goldprice.dev

Alpha Vantage has been removed.

## Data
- Live XAU/USD: goldprice.dev `/v1/prices`
- Historical XAU/USD: goldprice.dev `/v1/bars`
- Free historical window: latest 30 days
- `GOLDPRICE_API_KEY` is optional; anonymous requests work for initial use.

## .env
GOLDPRICE_API_KEY=
GEMINI_API_KEY=YOUR_GEMINI_KEY
GEMINI_MODEL=gemini-3.6-flash

## Run
python -m pip install -r requirements.txt
python -m streamlit run app.py

The generated gold background remains bundled in `assets/gold-background.png`.


## V9.1
Fixed CSS stacking so the dark overlay affects only the generated gold background, not text, cards, tabs, or charts.

## V10 — Firebase Authentication
Adds Email/Password Register, Login and Logout using Firebase Authentication REST API.

Streamlit Secrets / local `.env`:

FIREBASE_API_KEY="..."
GOLDPRICE_API_KEY="..."   # optional
GEMINI_API_KEY="..."
GEMINI_MODEL="gemini-3.6-flash"

Firebase Console must have Authentication > Sign-in method > Email/Password enabled.
