# Project Development Guidelines

## 1. Implementing the Menu

### Step 1.1

- Create a string for the menu showing 3 options
- Get the users choice as an int and print a message for each option(if statement)
- Test and Run

### Step 1.2

- Add a while loop so that the user can exit loop on choosing `3`
- Hint: Easiest way is forever loop + if statement + break
- Test and Run

## 2. Implementing "Option 1": Adding Performers

### Step 2.1

- Get the number of performers to be addded from the user
- Add a counting loop for this ie. printing `1/3`, `2/3`, `3/3` if they type in `3`.
- Test and Run

### Step 2.2

- Add code to get information about each performer that needs to be added
- Get the first name and surname
- Get the type of performance - as a number
- Get the length of the performance - as a number
- Add an if statement to initialise a string for `performance_type` to be `Dancer`/`Singer`/`Musician`.
- Create a variable using f-string containing the details for a performer. ie `Ann Ford Musician 20 minutes`
- Print this variable in the loop for testing.
- Test and Run

### Step 2.3

- Create a string accumulator variable for all the performers details.
- In your loop add the line of information about each performer to this variable
- Modify the program so there is a single print statement that shows the information for all performers once all the data for this set of performers has been added

### Step 2.4

- Add counters for
  - no. of musicians
  - no. of singers
  - no. of dancers
  - total time
- Set these variables to `0` before the loop and bump up when appropriate ( you may need to add if statements)
- print these outside the loop. ie once all of this set of performers have been added
- convert the total minutes to hours and minutes

### Step 2.5

- Create an empty file `performer.txt` in the same directory as your program in pycharm.
- At the start of “Add Performers” open the file to append to the file.
- Add 1 line to the file for each performer: create a line of data that matches the format of the data stored in the file
- Once a set of performers have been added close the file
- Test and Run

## Implementing "Option 2": Generating Concert Schedule

### Implementation Details

The program has been implemented in Python and makes use of:

- File I/O operations for storing performer details
- Data validation to ensure proper input
- String formatting for consistent output
- Error handling for invalid inputs
- Data transformation for displaying statistics

### Key Components

1. **Main Menu Loop**: Continuously shows options until the user chooses to quit
2. **Performer Input**: Collects and validates performer details
3. **File Handling**: Reads and writes to the `performer.txt` file
4. **Statistics Calculation**: Computes performance metrics
5. **Output Formatting**: Displays information in a user-friendly way

### Error Handling

The program provides appropriate error messages for:

- Invalid menu selections
- Non-numeric inputs where numbers are required
- Invalid performance type selections
- Non-positive performance durations

### Data File Format

The `performer.txt` file uses a simple space-separated format:

```plaintext
LastName FirstName PerformanceType Duration
```

## Technical Implementation

The program is structured as follows:

1. **Main Menu** - Provides user interface for choosing operations
2. **Performer Management** - Handles adding new performers and saving to file
3. **Schedule Generation** - Reads performer data and creates formatted output

## Development Notes

- The program handles various input validation scenarios
- Performer data is persisted between program runs
- Statistics are calculated for each batch of added performers
