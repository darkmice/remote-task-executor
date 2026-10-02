# Remote task executor

This public repository contains only a generic GitHub Actions launcher and a pinned browser dependency. The executable task code is retrieved at run time from an authenticated control endpoint. Actions secrets are configured only on the original repository; copied repositories cannot access the task code or control API.

GitHub still publishes workflow metadata, step names, status, and timing. The application redirects stdout and stderr and sends task results to the control API. No task output is uploaded as an Actions artifact.
