# YAML Notes

## What is YAML?
YAML (Yet Another Markup Language) is a way to structure data in a readable format. It's used a lot in config files and data exchange between systems.

### YAML vs. Other Formats
Same data written in XML, JSON, and YAML:

**XML:**
```xml
<servers>
    <server>
        <name>Server1</name>
        <ip>192.168.1.1</ip>
    </server>
</servers>
```

**JSON:**
```json
{
    "servers": [
        {
            "name": "Server1",
            "ip": "192.168.1.1"
        }
    ]
}
```

**YAML:**
```yaml
servers:
  - name: Server1
    ip: 192.168.1.1
```
YAML is easier to read and work with compared to XML and JSON.

---

## YAML Basics
### 1. Key-Value Pairs
Basic data representation in YAML:
```yaml
Fruit: Apple
Vegetable: Carrot
Liquid: Water
Meat: Chicken
```
**Rules:**
- Key and value are separated by `:` and a space.
- Indentation needs to be consistent.

### 2. Lists (Arrays)
Lists use dashes (`-`).
```yaml
Fruits:
  - Apple
  - Banana
  - Orange
```
**Rules:**
- A key followed by a colon defines the list.
- Each item in the list starts with a `-`.

### 3. Dictionaries (Maps)
A dictionary groups key-value pairs together.
```yaml
Banana:
  Color: Yellow
  Taste: Sweet
  Price: 0.50
```
**Rules:**
- Keep indentation consistent.
- Keys should align properly.

### 4. Nested Data
Lists and dictionaries can be combined.

**List of Dictionaries:**
```yaml
Cars:
  - Name: Toyota
    Year: 2022
    Color: Blue
  - Name: Honda
    Year: 2023
    Color: Red
```

**Dictionary Containing a List:**
```yaml
Person:
  Name: John Doe
  Hobbies:
    - Reading
    - Hiking
    - Coding
```

---

## Formatting Rules
- **Indentation matters:** Always use consistent spaces.
- **No tabs:** YAML only allows spaces.
- **Dictionaries are unordered:** The order of key-value pairs doesn’t matter.
- **Lists are ordered:** Positioning matters.
- **Comments start with `#`:**
```yaml
# This is a comment
Fruit: Apple  # Another comment
```

---

## Summary
- YAML is used for storing and structuring data.
- Supports **key-value pairs**, **lists**, and **dictionaries**.
- Indentation and spacing must be correct.
- Lists are ordered, dictionaries are not.
- Common in cloud computing, DevOps, and automation.

