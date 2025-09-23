# Adventurers’ Guild Registry

Welcome, traveler! To join the Guild and begin your quest:

## How to enroll
1. Fork this repository to your own account.
2. **Create a NEW file** at `teams/<team-slug>.yml` (kebab-case).
3. Copy the template below into your file and fill it in.
4. Open a Pull Request back to this repo.

**IMPORTANT**: Only create NEW files in the `teams/` directory. Do not modify any existing files!

When your PR passes the trials, the Guild Scribe will write you into the book of legends and register your party. You’ll then receive your **Guild Mark**

### Template
```yaml
team_name: "Gilded Griffons"
team_slug: "gilded-griffons"   # must match filename
captain:
  name: "Ayla Brass"
  contact: "signal:@ayla"      # handle only; no phone numbers
members:
  - "Jax"
  - "Mira"
  - "Thorn"
pledge: "We shall not test beyond the dungeon walls."
```
## Rules
- By submitting you are concenting to logging for the purpouse of scoring (only while on your quest) No logging will be active outside of the trials.
- Keep it clean
- Only one guild may be registered per person. No bots.
- **Edits are allowed before merge, but once your team is registered, the record is permanent.**

## What NOT to modify
**Your PR will be automatically rejected if you modify any of these protected files:**
- `.github/` - Workflow files and templates
- `schemas/` - Validation rules
- `README.md` - These instructions
- `teams/example-guild.yml` - Example template

**What you CAN do:** Create a NEW file at `teams/<your-team-slug>.yml`


---

## 🗝️ The Trial of the Guild Mark

*"Once the Guild Scribe has inscribed your name in the ancient ledger, your true test begins..."*

The Guild Mark is not simply given—it must be **claimed** by those clever enough to decipher the Scribe's riddle. Only adventurers who demonstrate both technical prowess and wit shall proceed to the next trial.

### The Scribe's Riddle

*Listen well, for the Scribe speaks in whispers:*

> *"The guild-registry-worker dwells in the realm of where media was once hosted,
> Seek the path of 'guild-mark' with your team's true name within.
> The ancient protocol of 'team=' shall be your key,
> To unlock the mark that sets your spirit free."*

*The wise know that some paths require no sorcery—merely the right incantation spoken to the correct oracle.*

### For the Truly Lost

*Should you find yourself wandering in darkness, remember:*
- The **Scribe's domain** is known to those who read carefully
- Your **team's true name** is the slug you chose with care
- The **ancient protocol** has been used since the dawn of the web
- **No authentication** guards this knowledge—it is freely given to those who seek

*May your queries be swift and your responses be JSON.*

---

*The Guild Scribe validates all submissions automatically. Your team file will be checked against the schema in `schemas/team.schema.json`.*