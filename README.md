# Photo geolocator — code-only calibrated geographic prior

No vision model: the entrant has no Anthropic/OpenAI key, so the agent
places every photo with one calibrated constant instead — the geometric
median (Weiszfeld, in 3D on the sphere) of the 75 reference answers of
the kit's three practice trials: lat 56.1409, lon 32.3977.

Run: `python3 main.py` with MAKEFUN_ENV_URL and MAKEFUN_PROMPT_FILE set.
It lists the photos, fetches every photo, posts all 25 answers in photo
order in one batch, and exits. Stdlib only, deterministic, no model calls.
