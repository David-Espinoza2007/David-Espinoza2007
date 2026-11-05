# David Espinoza

I'm studying Ingeniería en Tecnologías Computacionales at Tecnológico de Monterrey in Mexico. My work includes AI agents, client websites, Python applications, and C++ coursework.

## Hardware substitution assistant

**[datathon-emerson-sustitutos](https://github.com/DummkoffLad/datathon-emerson-sustitutos)**

**1st place, Datathon MICAI 2026**: winner of the *Asistente agéntico para reemplazo de hardware especializado* challenge, set by Emerson. The datathon was organized by the Sociedad Mexicana de Inteligencia Artificial and Tecnológico de Monterrey, with Databricks as sponsor.

The assistant takes a discontinued part, or a plain-language description of what is needed, and recommends active substitutes from the catalog. For each one it gives the price, the stock and a short explanation, and it builds the quote. I built the functional side:

- a deterministic matching engine that grades each substitute and checks every recommendation against the datasheets;
- an agent with tools, running on the Databricks LLM, for technical and inventory questions, with a verifier that rejects quotes and figures not found in the sources;
- a chat app in Streamlit with follow-up memory, multi-part questions and quantities capped at stock;
- an evaluation suite that runs the real app with every switch combination.

**Stack:** Python, Streamlit, Databricks (Foundation Model API, Unity Catalog, Vector Search, MLflow).

## Web development

I built the following websites using **Next.js (React), Tailwind CSS, and Vercel**, with Claude as a development assistant.

**+Pacientes — project work, 2026**

- **[Dr. Hugo Adrián Sánchez Calvario](https://dr-hugo-sanchez-calvario.vercel.app/)** — an orthopedic surgeon's website in Puerto Vallarta with Google reviews, a video story, treatments by condition, 24-hour emergency contact, and embedded appointment scheduling.
- **[Dr. Jorge Álvaro González Ross](https://jorge-alvaro-gonzalez-ross.vercel.app/)** — an endoscopic spine surgeon's website in Guadalajara with procedure information, international training, video content, patient reviews, and a scheduling dialog.

The medical sites integrate +Pacientes scheduling, Google Maps, and WhatsApp contact links.

## Earlier projects

- **[Vaccine cold-chain monitoring](https://github.com/David-Espinoza2007/entregable_01)** — LoRaWAN temperature monitoring for vaccines.
- **[Piano roadmap](https://github.com/David-Espinoza2007/piano-roadmap)** — a piano learning roadmap as an installable PWA.
- **[Search and sorting algorithms](https://github.com/David-Espinoza2007/Act-1.2-Algoritmos-de-Busqueda-y-Ordenamiento)** — C++ coursework.
