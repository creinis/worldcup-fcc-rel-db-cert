# World Cup Database Queries

###### Technologies:
<p align="center">
<img src="https://img.icons8.com/color/75/000000/console.png" width="75" height="75" alt="Bash" style="margin: 10px 15px 0 15px;" />
<img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/skills/postgresql-colored.svg" width="75" height="75" alt="PostgreSQL" style="margin: 10px 15px 0 15px;" />
</p>

- **Bash:** Used for writing shell scripts that facilitate interaction with the World Cup database.
- **PostgreSQL:** Relational database management system used to store data about teams, games, and goals.

### Try it!

To run the World Cup database queries, follow the instructions in the Setup section below.

### Functionality

This project demonstrates various queries to extract insights from a World Cup database. The PostgreSQL database stores information about games and teams, while the bash script facilitates interaction with the database.

## Project Structure

- `worldcup.sql`: Contains the SQL script to create and populate the PostgreSQL database.
- `queries.sh`: Bash script that executes a series of queries to extract data from the database.

## Setup

### Prerequisites

- PostgreSQL installed
- Bash shell

### Installation Steps

1. Clone the repository:
   ```bash
   git clone https://github.com/creinis/world-cup-database.git
   cd world-cup-database
   ```

2. Create the PostgreSQL database and tables:
   ```bash
   psql -U postgres -f worldcup.sql
   ```

3. Make the bash script executable:
   ```bash
   chmod +x queries.sh
   ```

4. Run the bash script to execute the queries:
   ```bash
   ./queries.sh
   ```

## Practical Use Case

This project can be used to analyze World Cup data and extract useful statistics and insights. The command-line interface simplifies interaction with the system, while the PostgreSQL database ensures structured data storage.

## Benefits

- **Structured Data Management:** Organizes information about teams and games into relational tables for efficient querying.
- **Simple Interaction:** Bash scripts provide an intuitive command-line interface to execute predefined queries.
- **Ease of Maintenance:** SQL and bash scripts simplify initial setup and ongoing maintenance of the system.
- **Extensibility:** Potential for future expansion with new queries, additional data, or integration with other tools for data analysis.

---

#### This is a FreeCodeCamp Challenge for Relational Database Projects Certification
<p align="center">
<img src="https://cdn.freecodecamp.org/platform/universal/fcc_primary.svg" width="250" height="75" alt="freeCodeCamp" style="margin: 0 15px; opacity: 0.6" />
</p>

---

## Output

When you run the `queries.sh` script, you will see the following output:

```bash
Total number of goals in all games from winning teams:
68

Total number of goals in all games from both teams combined:
90

Average number of goals in all games from the winning teams:
2.1250000000000000

Average number of goals in all games from the winning teams rounded to two decimal places:
2.13

Average number of goals in all games from both teams:
2.8125000000000000

Most goals scored in a single game by one team:
7

Number of games where the winning team scored more than two goals:
6

Winner of the 2018 tournament team name:
France

List of teams who played in the 2014 'Eighth-Final' round:
Algeria
Argentina
Belgium
Brazil
Chile
Colombia
Costa Rica
France
Germany
Greece
Mexico
Netherlands
Nigeria
Switzerland
United States
Uruguay

List of unique winning team names in the whole data set:
Argentina
Belgium
Brazil
Colombia
Costa Rica
Croatia
England
France
Germany
Netherlands
Russia
Sweden
Uruguay

Year and team name of all the champions:
2014|Germany
2018|France

List of teams that start with 'Co':
Colombia
Costa Rica
```
