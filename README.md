# YAML Notes

## What is YAML?
YAML (Yet Another Markup Language) is a structured, human-readable format used for configuration files and data exchange.

## YAML Syntax

### 1. Key-Value Pairs
```yaml
Fruit: Apple
Vegetable: Carrot
Liquid: Water
Meat: Chicken
```
- Key and value are separated by a `:` and a space.
- Indentation must be consistent.

### 2. Lists (Arrays)
```yaml
Fruits:
  - Apple
  - Banana
  - Orange
```
- Lists are indicated using a `-` before each item.

### 3. Dictionaries (Maps)
```yaml
Banana:
  Color: Yellow
  Taste: Sweet
  Price: 0.50
```
- Groups related key-value pairs.

### 4. Nested Structures
YAML allows nesting of lists and dictionaries.
```yaml
Cars:
  - Name: Toyota
    Year: 2022
    Color: Blue
  - Name: Honda
    Year: 2023
    Color: Red
```
```yaml
Person:
  Name: John Doe
  Hobbies:
    - Reading
    - Hiking
    - Coding
```

## Formatting Rules
- **Use spaces, not tabs**.
- **Dictionaries are unordered**, lists are ordered.
- **Comments start with `#`**:
```yaml
# This is a comment
Fruit: Apple  # Another comment
```

---
This covers general YAML. For Kubernetes YAML, see [`kubernetes-yaml.md`](./kubernetes-yaml.md).
