# Get-DirectorySize

A terminal command that recursively measures the size of a directory and it's children.

## Usage

The following implementation logs all child items in the current directory and sorts them from largest to smallest, only showing the top 5.

```bash
Get-DirectorySize -Depth 1 -ExcludeSelf |
Sort-Object Size -Descending |
Select-Object -First 5
```

## Credit

mklement0 on [StackOverflow](https://stackoverflow.com/a/54297192)
