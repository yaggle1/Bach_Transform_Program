# Bach Transform Program - Project Context

## Overview
The Bach Transform Program is an innovative tool that automates the creation of pedagogical arrangements of J.S. Bach's works. Created by TMLavios, this program transforms complex Bach pieces into progressive learning arrangements while preserving Bach's essential musical elements.

## Core Concepts

### Analytical Arrangements (AAs)
- Progressive versions of Bach pieces with different rhythmic complexities
- Naming convention: RxLy where:
  - R = Right hand (Treble clef)
  - L = Left hand (Bass clef)
  - x,y = note duration (2=half, 4=quarter, 8=eighth, 16=sixteenth)

### Transformation Sequence
Most complex to simplest:
1. R16L8 (Original/final form)
2. R8L8
3. R4L8
4. R8L4
5. R4L4
6. R2L4
7. R4L2
8. R2L2 (Simplest form)

## Project Structure
```
Bach_Transform_Program/
├── src/
│   └── bach-transform.py
├── examples/
│   ├── suites/
│   │   ├── suite2/
│   │   │   └── allemande/
│   │   ├── suite4/
│   │   │   └── allemande/
│   │   └── suite5/
│   │       └── bouree/
│   └── wtc/
│       └── fugue3/
├── docs/
│   ├── bach-transform-doc.md
│   ├── transformation-doc.md
│   └── git-cheatsheet.md
└── lib/
    └── base_musicxml/
```

## Technical Implementation
- Uses music21 library for MusicXML processing
- Python-based transformation engine
- Git/GitHub for version control
- Preserves:
  - Pitch content
  - Voice leading
  - Measure boundaries
  - Time signatures

## Current Status
- Repository: https://github.com/yaggle1/Bach_Transform_Program
- Branch structure:
  - master: Stable releases
  - development: Active development
- Working transformation: R16L8 → R2L2

## Musical Goals
1. Preserve Bach's musical integrity while simplifying rhythm
2. Maintain voice leading and harmonic structure
3. Create pedagogically sound progression of arrangements
4. Support systematic learning of complex pieces

## Development Goals
1. Complete transformation engine for all arrangement types
2. Add support for various Bach works
3. Implement robust testing
4. Create user-friendly interface
5. Document pedagogical approach

## Current Files
- Working example: Suite 5 Bourée
  - R16L8_A.musicxml (complex version)
  - R2L2_A.musicxml (simplified version)

## Technical Notes
1. Uses semantic versioning (MAJOR.MINOR.PATCH)
2. Follows PEP 8 style guide
3. Requires Python 3.8+
4. Uses conventional commit messages

## Key Algorithms
1. Rhythmic simplification while preserving:
   - First pitch from each group
   - Strong beats
   - Voice leading
2. Measure boundary preservation
3. Time signature maintenance

## Next Steps
1. Complete transformation pipeline
2. Add more test cases
3. Implement additional arrangement types
4. Enhance documentation

## References
- Original creator: TMLavios
- Technical support: Claude
- Version control: Git/GitHub
- Primary library: music21

This context represents the Bach Transform Program as of February 2025.
