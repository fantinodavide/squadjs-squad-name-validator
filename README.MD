## SquadNameValidator
Squad Name Validator plugin for SquadJS.
Automatically disbans squads if their name is not compliant to specific rules.
Every rule is CASE-INSENSITIVE

### Example configuration
```json
{
    "plugin": "SquadNameValidator",
    "enabled": true,
    "rules": [
        {
            "type": "regex",
            "rule": "[^a-z0-9\\=\\[\\]\\!\\.\\s]"
        }
    ]
}
```
