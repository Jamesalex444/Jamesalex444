import random

# Function to generate combinations
def generate_combinations():
    combinations = []
    while len(combinations) < 300:
        combination = sorted(random.sample(range(1, 40), 5))
        if combination not in combinations:
            combinations.append(combination)
    return combinations

# Generate combinations
combinations = generate_combinations()

# Print combinations
for i, combination in enumerate(combinations, 1):
    print(f"{i}: {combination}")
