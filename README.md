# David Espinoza

I'm studying Ingeniería en Tecnologías Computacionales at Tecnológico de Monterrey in Mexico. My work includes AI agents and client websites.

## Hardware substitution assistant

**[datathon-emerson-sustitutos](https://github.com/DummkoffLad/datathon-emerson-sustitutos)**

**1st place, Datathon MICAI 2026**: winner of the *Asistente agéntico para reemplazo de hardware especializado* challenge, set by Emerson. The datathon was organized by the Sociedad Mexicana de Inteligencia Artificial and Tecnológico de Monterrey, with Databricks as sponsor.

The assistant takes a discontinued part, or a plain-language description of what is needed, and recommends active substitutes from the catalog. For each one it gives the price, the stock and a short explanation, and it builds the quote. I built the functional side:

- a deterministic matching engine that grades each substitute and checks every recommendation against the datasheets;
- an agent with tools, running on the Databricks LLM, for technical and inventory questions, with a verifier that rejects quotes and figures not found in the sources;
- a chat app in Streamlit with follow-up memory, multi-part questions and quantities capped at stock;
- an evaluation suite that runs the real app with every switch combination.

**Stack:** Python, Streamlit, Databricks (Foundation Model API, Unity Catalog, Vector Search, MLflow).

## Wildfire record across satellites

**[fire-pulse](https://github.com/David-Espinoza2007/fire-pulse)** · live map: **[Blaze Bridge](https://blazebridge-map.hf.space)**

Team project for the **NASA Space Apps Challenge 2026**, challenge *Harmonization of MODIS and VIIRS Hot Spots*. When newer fire satellites arrived in 2012 and 2018, the yearly fire counts jumped several times over even though there was not that much more fire. Blaze Bridge puts 25 years of NASA FIRMS detections on one comparable scale, using about 50,000 conversion factors by region, season and time of day, so any country, state or drawn area can be checked against its own normal.

I worked on both the technical side and the interface:

- the harmonization method with my teammate: the conversion between the older and newer satellites, its validation on hidden years, and the data pipeline;
- a globe and flat map in d3 with three looks, fire drawn by detection density, and zoom down to single 375 m detections;
- two modes: a clean Presentation view and a Research view with tools for area selection, time ranges, playback and filters;
- an analysis panel with the fire calendar, the season compared with past years, validation notes and data downloads;
- the pitch deck and the live demo.

**Stack:** Python, DuckDB, FastAPI, D3, Hugging Face Spaces. Data: NASA FIRMS (MODIS C6.1, VIIRS 375 m).

## Web development

I built the following websites using **Next.js (React), Tailwind CSS, and Vercel**, with Claude as a development assistant.

**+Pacientes — project work, 2026**

- **[Dr. Hugo Adrián Sánchez Calvario](https://dr-hugo-sanchez-calvario.vercel.app/)** — an orthopedic surgeon's website in Puerto Vallarta with Google reviews, a video story, treatments by condition, 24-hour emergency contact, and embedded appointment scheduling.
- **[Dr. Jorge Álvaro González Ross](https://jorge-alvaro-gonzalez-ross.vercel.app/)** — an endoscopic spine surgeon's website in Guadalajara with procedure information, international training, video content, patient reviews, and a scheduling dialog.

The medical sites integrate +Pacientes scheduling, Google Maps, and WhatsApp contact links.
