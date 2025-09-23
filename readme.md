# LB 324

## Aufgabe 2
Erklären Sie hier, wie man `pre-commit` installiert.

- Installation von pre-commit:

    pre-commit installieren

      # Windows
      pip install pre-commit

      # macOS
      pip3 install pre-commit

- Konfigurationsdatei erstellen:
    Danach legt man im Projekt eine Datei .pre-commit-config.yaml an.
    Beispiel für einen Hook, der bei jedem Commit die Tests ausführt:
    
    repos:
      - repo: local
      hooks:
      - id: pytest-check
        name: pytest-check
        entry: python3 -m pytest
        language: system
        types: [python]
        stages: [commit]
        pass_filenames: false
        always_run: true

- Hooks aktivieren

  Im Terminal oder in der PowerShell werden die Hooks mit folgendem Befehl installiert:

  pre-commit install --hook-type pre-commit --hook-type pre-push

  
## Aufgabe 4

Erklären Sie hier, wie Sie das Passwort aus Ihrer lokalen `.env` auf Azure übertragen.

<img width="1906" height="404" alt="image" src="https://github.com/user-attachments/assets/24c35d95-cd0d-438b-8f4a-3423de5b1167" />

https://fiddenfast-aufxcscqa6bheqen.francecentral-01.azurewebsites.net/


