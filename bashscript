#!/usr/bin/env bash

# Function to count files
function file_count {
    echo $(ls -1 | wc -l)
}

# Actual number of files in current directory
correct=$(file_count)

echo "Welcome to the Guessing Game!"
echo "How many files are in the current directory?"

# Loop until user guesses correctly
while true; do
    read -p "Enter your guess: " guess
    if [[ $guess -eq $correct ]]; then
        echo "🎉 Congratulations! You guessed correctly."
        break
    elif [[ $guess -lt $correct ]]; then
        echo "Too low. Try again."
    else
        echo "Too high. Try again."
    fi
done
