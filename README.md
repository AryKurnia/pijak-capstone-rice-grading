# pijak-capstone-rice-grading
Rice quality grading system using custom CNN to classify rice images into Good, Medium, and Poor categories. Built with TensorFlow/Keras, Python, and Node.js web interface.

## Struktur
  ```txt
  pijak-capstone-rice-grading/
  ├── api/                        # Hapi.js REST API
  │   ├── src/
  │   │   ├── routes/
  │   │   ├── handlers/
  │   │   └── plugins/
  │   ├── package.json
  │   └── .env.example
  │
  ├── inference/                  # Flask + TF inference service
  │   ├── app/
  │   │   ├── model/              # SavedModel / .h5 disini
  │   │   └── routes/
  │   ├── requirements.txt
  │   └── .env.example
  │
  ├── frontend/                   # Web frontend
  │   └── ...
  │
  ├── docs/                       # Swagger spec, arsitektur, dll
  │   └── swagger.yaml
  │
  ├── .gitignore
  ├── README.md
  └── docker-compose.yml          # Orchestrate semua service
  ```

## How to run
```bash
  # Build
  docker compose build

  # Jalankan
  docker compose up -d

  # Cek log
  docker compose logs -f inference

  # Stop
  docker compose down
```
