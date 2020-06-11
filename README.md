# Workspace_Utils 

## Keeping your connection alive during long processes
Workspaces automatically disconnect when the connection is inactive for about 30 minutes, which includes inactivity while deep learning models are training. You can use the workspace_utils.py module here to keep your connection alive during training. The module provides a context manager and an iterator wrapper—see example use below.

*NOTE:* The script sometimes raises a connection error if the request is opened too frequently; just restart the jupyter kernel & run the cells again to reset the error.

*NOTE:* These scripts will keep your connection alive while the training process is running, but the workspace will still disconnect 30 minutes after the last notebook cell finishes. Modify the notebook cells to save your work at the end of the last cell or else you'll lose all progress when the workspace terminates.

### Source: Udacity
