## Backend

Install dependencies:

```bash
pip install -r requirements.txt
```

Run backend:

```bash
uvicorn main:app --reload
```

Backend runs on:

```txt
http://localhost:8000
```

---


# DAG Validation

Integrated backend pipeline validation.

The backend:
- parses node/edge structure
- counts nodes and edges
- validates whether the graph is a valid DAG

Example response:

```json
{
  "num_nodes": 5,
  "num_edges": 4,
  "is_dag": true
}
```

---
