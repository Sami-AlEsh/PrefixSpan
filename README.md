# PrefixSpan
PrefixSpan algorithm implementation using Python.

## Quick Start

This simple python script **does not rely on any other third-party libraries**. Just confirm that your environment is **Python 3**.

## Simple Demo
```python
sample_data = [
    ['C', 'A', 'G', 'A', 'A', 'G', 'T'],
    ['T', 'G', 'A', 'C', 'A', 'G'],
    ['G', 'A', 'A', 'G', 'T']
]

patterns = dict()
PrefixSpan(sample_data, min_support=3)
```

```python
print('Patterns:', patterns)
plot_result(patterns.keys(), patterns.values(), 'Patterns Support Visualization', 'pattern', 'support')
```

### Results:
> Patterns: {'^T': 3, '^G': 3, '^A': 3, 'G^A': 3, 'G^G': 3, 'GA^A': 3, 'GA^G': 3, 'GAA^G': 3, 'A^A': 3, 'A^G': 3, 'AA^G': 3}

**Note:** '^' is a separator character between items.
