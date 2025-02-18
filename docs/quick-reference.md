# Bach Transform Program - Quick Reference

## Transformation Types
```
Most Complex → Simplest
R16L8 → R8L8 → R4L8 → R8L4 → R4L4 → R2L4 → R4L2 → R2L2

R = Right hand (Treble)
L = Left hand (Bass)
Numbers = Note duration (2=half, 4=quarter, 8=eighth, 16=sixteenth)
```

## Key Files Location
```
/examples/suites/suite5/bouree/
    ├── Ste5_Bouree_R16L8_A.musicxml
    └── Ste5_Bouree_R2L2_A.musicxml
```

## Main Git Commands
```bash
git checkout development     # Switch to development branch
git status                  # Check file status
git add .                   # Stage changes
git commit -m "type: msg"   # Commit changes
git push                    # Upload to GitHub
```

## Core Transformation Rules
1. Preserve first pitch from each group
2. Maintain measure boundaries
3. Keep voice leading intact
4. Respect time signatures

## Project Structure
```
Bach_Transform_Program/
├── src/           # Python code
├── examples/      # MusicXML files
├── docs/          # Documentation
└── lib/           # Shared resources
```

## Common Operations
```python
# Transform a piece
transformer = BachTransformer()
transformer.transform_R16L8_to_R2L2(
    "input.musicxml",
    "output.musicxml"
)
```

## Repository
- URL: github.com/yaggle1/Bach_Transform_Program
- Main branch: master (stable)
- Development: development branch

## Quick Start
1. Switch to development branch
2. Pull latest changes
3. Make modifications
4. Commit with descriptive message
5. Push to GitHub

## Contact
- Author: TMLavios
- Support: Claude
