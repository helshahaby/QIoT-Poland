# QPoland — Production Scheduling Optimization

## Deliverables
- `QPoland_Production_Scheduling.ipynb` — Google Colab notebook.
- `QPoland_Production_Scheduling.pptx` — six-slide pitch deck.
- `QPoland_Production_Scheduling_Demo.mp4` — animated Gantt-style demo.
- Notebook generates `schedule_2x2.json` and `schedule_3x3.json`.

## Run
1. Upload the notebook to Google Colab.
2. Run cells top-to-bottom.
3. Download both JSON files from the final cell.

## Important assumptions
The screenshots specify machine routing and the mandatory instance sizes but do not include a numeric processing-time matrix or a formal JSON schema. The notebook therefore labels processing times as demo values and uses a clear, auditable JSON schema. Replace durations and adjust field names to the organizer's exact challenge specification if those details are provided.

## Solver honesty
The tiny required instances are solved with exact enumeration, which acts as a correctness oracle. Optional simulated annealing and OR-Tools CP-SAT comparison cells are included. The assignment QUBO is a compact sequencing subproblem; it is not presented as a full time-indexed QUBO for the entire schedule. No quantum advantage is claimed.
