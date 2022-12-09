## SquadNameValidator
Squad Name Validator plugin for SquadJS.
Automatically disbans squads if their name is not compliant to specific rules.
Every rule is CASE-INSENSITIVE

### Example configuration
```json
{
    "plugin": "SquadNameValidator",
    "enabled": true,
    "warningMessage": "Your squad has been disbanded due to non-compliant name.\n\nForbidden: %FORBIDDEN%",
    "rules": [
        {
            "type": "regex",
            "rule": "[^a-z\\d=\\$\\[\\]\\!\\.\\s\\-]"
        },
        {
            "type": "equals",
            "rule": "ARMOUR"
        },
        {
            "type": "includes",
            "rule": "F*CK"
        }
    ]
}
```
