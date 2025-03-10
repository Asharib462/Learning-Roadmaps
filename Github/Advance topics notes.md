# Advanced Git Topics

- **git reflog**: Maintains all the history of the changes made to the branch and commits, even the actions that are related to the commit such as resetting the branch.

- **git bisect**: Allows you to identify the commit that introduces a bug.

- **git worktree**: Allows you to work on multiple directories at the same time, without stashing the changes in the current branch.

- **git attributes**: Store the settings in the `.gitattributes` file, controlling how git handles the files in the repository.

- **git LFS**: Large File Storage, allows you to store large files by tracking metadata, not storing the entire files. It allows storing and tracking binary assets such as images, videos, and audio files separately from your regular git repository. *Note: Git LFS requires a separate server or storage system to store actual files.*
