# Blackwater Concert Organizer

<img src="https://marketing.mtu.ie/contentfiles/images/MTU/Logos/MTU_Logo_Colour_RGB_300dpi.jpg" alt="Cork Institute of Technology" width="250px" />

**SOFT6018 Programming Fundamentals Project**

## Overview

This program helps organize the Blackwater Annual Concert by managing performer details and generating a concert schedule. The program stores performer information in a text file and can display concert details based on that data.

## Features

The program offers two main options:

1. **Adding Performers** - Add new performers to the concert
2. **Generate Concert Details** - Display the finalized concert schedule

## Usage Instructions

### Adding Performers

When adding performers, you'll need to provide:

- First name and last name
- Type of performance (Musical, Singer, or Dance)
- Duration of performance in minutes

After performers are added, a summary is displayed showing:

- Individual performer details
- Number of musicians, singers, and dancers
- Total performance time
- Longest act information

### Generating Concert Details

This feature reads the stored performer data and displays a formatted concert schedule. Performances longer than 15 minutes are marked with an asterisk (*).

## Data Storage

All performer information is stored in a file called `performer.txt` with the following format:

```plaintext
LastName FirstName PerformanceType Duration
```

## Example Usage

### Adding Performers

```plaintext
Blackwater Annual Music Concert
-------------------------------
1. Adding Performers
2. Generate Concert Details
3. Quit
==> 1

(1) Adding Performers
---------------------
How many performers are you adding? 3

Booking 1/3:
Enter your name: Fred
Enter your surname: Walsh
Type of Performance
1. Musical
2. Singer
3. Dance
==> 1
Time slot required (mins): 15

Booking 2/3:
Enter your name: Harry
Enter your surname: Ford
Type of Performance
1. Musical
2. Singer
3. Dance
==> 3
Time slot required (mins): 25

Booking 3/3:
Enter your name: Sam
Enter your surname: Murphy
Type of Performance
1. Musical
2. Singer
3. Dance
==> 1
Time slot required (mins): 20

The following information has been added.

1. Walsh, Fred  Musician      15 minutes
2. Ford, Harry  Dancer        25 minutes
3. Murphy, Sam  Musician      20 minutes

Summary Notes:
--------------
2 Musician(s)
0 Singer(s)
1 Dancer(s)
Total time required: 1 hour(s), 0 min(s)
The longest act added is Harry Ford (Dancer) 25 minutes.
```

### Generating Concert Schedule

```plaintext
Blackwater Annual Music Concert
-------------------------------
1. Adding Performers
2. Generate Concert Details
3. Quit
==> 2

(2) Concert Details
--------------------
1: Fred Walsh  (Musician) 15 minutes
2: Harry Ford*  (Dancer) 25 minutes
3: Sam Murphy*  (Musician) 20 minutes
4: Mary Murphy*  (Dancer) 19 minutes
```

## Author

P Richard Szilagyi, 2020
