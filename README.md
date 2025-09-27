# Adventurers’ Guild Registry

Hear ye, hear ye! Brave traveller, you stand before the desk of the Guild Scribe. To be written into the Ledger and begin your saga, follow this quest.

## Act I — The Call to Adventure (Enrolment)
1. Fork this repository to your own account.
2. **Create a NEW file** at `teams/<team-slug>.yml` (kebab-case).
3. Copy the charter template below into your file and complete it truthfully.
4. Open a Pull Request back to this repository.
5. Wait for the Guild Scribe to validate your request and merge your PR.

## Act II — Forge Your Charter (The Team File)
- Your file name must be `teams/<team-slug>.yml`, where `<team-slug>` is kebab-case.
- The `team_slug` inside your document must exactly match the file name.
- The captain’s `contact` is a handle only (for example, `signal:@ayla`); no phone numbers.

### Example Charter Template
```yaml
team_name: "Gilded Griffons"
team_slug: "gilded-griffons"   # must match filename
captain:
  name: "Ayla Brass"
members:
  - "Ayla"
  - "Jax"
  - "Mira"
  - "Thorn"
pledge: "We shall not test beyond the dungeon walls."
```

## Act III — Trial I: Claim the Guild Mark
“Once the Guild Scribe has inscribed your name in the ancient ledger, your first trial begins.”

The Guild Mark is not simply given — it must be **claimed**. After your PR is merged and your party is registered, seek your mark by invoking the Scribe’s oracle:

- Call for the 'guild-registry-worker'
- At the domain where media once was found. Fun made of a larger streaming service.
- Speak to the path: `/guild-mark`
- Whisper your team’s true name as: `?team=<your-team-slug>`
- The response reveals your Guild Mark. Guard it well.

Those who read the signs carefully will know where the Scribe’s domain resides. No authentication wards this door; the correct query is key enough.

## Act IV — Guild Laws and Oaths
- By submitting, you are consenting to logging for the purpose of scoring during your quest. No logging is active outside the trials.
- Only one guild may be registered per person. No bots.
- Edits are allowed before merge, but once your team is registered, the record is permanent.
- Keep it clean.

## Act V — Forbidden Tomes (Do Not Modify)
Your PR will be automatically rejected if you modify any of these protected scrolls:
- `.github/` — Workflows and templates
- `schemas/` — Validation rules
- `README.md` — These instructions
- `teams/example-guild.yml` — Example template

What you CAN do: create a NEW file at `teams/<your-team-slug>.yml`.

---

## Behind the Curtain (How the Magic Works)
- The Guild Scribe validates every PR automatically against the rules and structure.
- When the PR is merged, the Guild registers your party and your first trial begins: claim your Guild Mark via the oracle described above.
- The schema for team files lives at `schemas/team.schema.json` should you wish to study it.

May your commits be steadfast and your responses swift.