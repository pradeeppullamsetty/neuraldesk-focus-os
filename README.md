# ✦ NeuralDesk — Focus Operating System

An intermediate-level productivity workspace built with Streamlit and Plotly. It pairs an Apple-inspired visual language with real task-management and focus workflows: glass-like panels, soft aurora lighting, a softly animated 3D-feeling orb, carefully tuned hover states, and responsive layouts.

## Features

- **Overview:** task snapshot, completion progress, open priorities, and a focused action board.
- **Task manager:** create, prioritize, filter, complete, clear, and export tasks as JSON.
- **Focus mode:** adjustable 15–60 minute Pomodoro-style sessions and a saved focus intention.
- **Insights:** interactive Plotly charts for task completion and projects.
- **No API key required.** The app runs with local/session data.
- **Reduced-motion support** and responsive spacing.

## Design inspiration

The engineering and design workflow was informed by [ECC](https://github.com/affaan-m/ECC) and its [frontend-design-direction skill](https://github.com/affaan-m/ECC/tree/main/skills/frontend-design-direction). This is a separate implementation; it does not package or copy ECC code or skills.

## Run locally

Python 3.10 or newer is recommended.

```bash
py -m pip install -r requirements.txt
py -m streamlit run app.py
```

If `py` is unavailable, use `python -m pip install -r requirements.txt` and `python -m streamlit run app.py`.

## Run tests

```bash
py -m pip install pytest
py -m pytest -q
```

## Deploy to Streamlit Community Cloud

1. Open https://share.streamlit.io/ and sign in with GitHub.
2. Select `pradeeppullamsetty/neuraldesk-focus-os`.
3. Set the main file path to `app.py`.
4. Click **Deploy**. No secrets are required.

## Data notes

Tasks and settings are held in the active Streamlit session, not a durable database. Export the task list as JSON to keep a backup. The focus timer is a lightweight session timer and runs while the app session is open.

## License

MIT
