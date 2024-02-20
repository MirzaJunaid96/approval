#!/bin/bash

input="### VERSION

4.2.0

### PATH

/home/ubuntu/uat/amneal/dwi

### BRANCH

platform-develop"

# Extract VERSION
version=$(echo "$input" | awk '/### VERSION/{flag=1; next} /###/{flag=0} flag' | tr -d '\n')

# Extract PATH
path=$(echo "$input" | awk '/### PATH/{flag=1; next} /###/{flag=0} flag' | tr -d '\n')

# Extract BRANCH
branch=$(echo "$input" | awk '/### BRANCH/{flag=1; next} /###/{flag=0} flag' | tr -d '\n')

echo "VERSION: $version"
echo "PATH: $path"
echo "BRANCH: $branch"
