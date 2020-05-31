## gh-label generate

Generate labels using a list

### Synopsis

This will generate labels using predefined label list or a custom
label file.

```
gh-label generate [flags]
```

### Examples

```
# Generate the labels using a predefined list
gh-label generate --repo erdaltsksn/playground --list "insane"

# User custom file as a list to generate the labels
gh-label generate --repo erdaltsksn/playground --file my-labels.json

# DANGER: Remove all the labels before generating the labels
gh-label generate --repo erdaltsksn/playground --list "insane" --force
```

### Options

```
      --file string   Use file as a label list. User --list "file.json"
  -f, --force         This will remove all labels before generate the labels.
  -h, --help          help for generate
  -l, --list string   Predefined label list name. Use --list "ABC"
  -r, --repo string   Repository which its labels will be exported into a file.
                      Please use 'username/repo-name' format.
```

### SEE ALSO

* [gh-label](gh-label.md)	 - This tool helps you generate labels for your Github repositories.

###### Auto generated by spf13/cobra on 30-May-2020