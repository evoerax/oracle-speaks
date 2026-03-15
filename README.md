# Oracle Speaks Skill

A comprehensive divination skill supporting multiple mystical traditions for guidance and insight.

## Overview

**Oracle Speaks** is a multi-method divination skill that provides guidance through:
- **I Ching (易经)**: The Book of Changes - ancient Chinese wisdom
- **Tarot Cards**: Western mystery tradition
- **Liu Yao (六爻)**: Six-line divination

## Features

- 🔮 **Multiple Divination Methods**
- 📊 **Rich Reference Materials**
- 🐍 **Python Scripts for Generation**
- 📱 **Single Machine / Offline Capable**
- 🌐 **Multi-language Support** (Chinese/English)

## Directory Structure

```
oracle-speaks/
├── SKILL.md              # Main skill instructions
├── README.md            # This file
├── scripts/             # Divination generators
│   ├── i_ching.py      # I Ching hexagram generator
│   ├── tarot.py        # Tarot card drawer
│   └── liu_yao.py      # Liu Yao generator
├── references/          # Interpretation guides
│   ├── i_ching_meanings.md
│   ├── tarot_cards.md
│   └── liu_yao_interpretations.md
└── evals/               # Test cases
    └── evals.json
```

## Usage

### I Ching Reading
```bash
python .skills/oracle-speaks/scripts/i_ching.py --method coin
```

### Tarot Reading
```bash
python .skills/oracle-speaks/scripts/tarot.py --cards 3 --positions past,present,future
```

### Liu Yao Reading
```bash
python .skills/oracle-speaks/scripts/liu_yao.py
```

### JSON Output
All scripts support `--json` flag for structured output:
```bash
python .skills/oracle-speaks/scripts/i_ching.py --json
```

## Triggering

This skill triggers when users mention:
- Divination, fortune-telling, guidance
- I Ching, Yijing, 易经
- Tarot, 塔罗牌
- Liu Yao, 六爻
- 占卜, 算卦, oracle, fate, destiny

## Examples

### Example 1: Career Decision
**User**: "I'm thinking about changing jobs, what should I do?"

**Response**: I Ching reading with hexagram interpretation and practical guidance

### Example 2: General Guidance
**User**: "What does the universe want me to know right now?"

**Response**: Divination reading with spiritual insight

### Example 3: Love Reading
**User**: "Draw 3 Tarot cards for my love life"

**Response**: Three-card spread with past/present/future interpretation

## Integration

This skill is designed to be used with AI assistants that support skill-based workflows. The skill provides:

1. **Generation Scripts**: Python scripts to generate divination symbols
2. **Reference Materials**: Comprehensive interpretation guides
3. **Structured Output**: Consistent format for readings

## Notes

- All calculations are local (no network required)
- Randomness uses Python's `random` module
- Readings are for entertainment and guidance purposes
- Always encourage professional advice for serious matters

## License

MIT