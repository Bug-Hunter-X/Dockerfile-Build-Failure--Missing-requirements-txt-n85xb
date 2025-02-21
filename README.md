# Dockerfile Bug: Missing requirements.txt

This repository demonstrates a common error in Dockerfiles: attempting to use a file (requirements.txt) that isn't present in the build context.

The initial `Dockerfile` attempts to install dependencies using `pip3 install -r requirements.txt`.  However, `requirements.txt` is not included in the build context, leading to a build failure.

The `Dockerfile_solution` demonstrates the corrected version, including the `requirements.txt` file in the build context.