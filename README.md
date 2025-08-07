# 🧠 Crosswizard

## 📌 Overview  
Crosswizard is a recursive puzzle-solving engine that takes a partially filled crossword grid and a word list, and attempts to fill in the grid with valid intersecting words. It's built for logic puzzle enthusiasts and developers interested in constraint-solving algorithms, showcasing efficient backtracking and pruning.

---

## 🚀 Features  
- ✅ Recursive backtracking engine for word placement  
- ✅ Smart pruning based on current board state  
- ✅ Support for custom grids and wordlists  

---

## 🛠️ Technologies Used  

| Area            | Stack/Tools                                   |
|-----------------|-----------------------------------------------|
| Backend         | Python                                        |

---

## 👨‍💻 My Role  
> Built the entire solving engine from scratch using Python.

- Designed and implemented a recursive backtracking algorithm  
- Heavily optimized performance by pruning invalid paths early (even the most complex of crosswords can be solved in milliseconds)
- Added support for dynamic grid parsing and custom word lists  

---

## 🧪 How to Run Locally

*Disclaimer: The input arguments for this engine are very complicated, and it's most likely pointless to try feeding it your own input. This repository only serves to display the specific methods used to optimize the performance of the engine.*

```bash
# Clone the repo
git clone https://github.com/IshanA2007/crosswizard.git
cd crosswizard

# (Optional) Create and activate a virtual environment
python -m venv venv
source venv/bin/activate  # or venv\Scripts\activate on Windows

# Run the solver 
python xwords2.py [dictionary file name] [test case]
# just so you know the bot works, here is one test case that you can run off the bat: python xwords2.py 20k.txt 8x9 14 V1x3E H5x0IGN# V0x3HERBS# V0x8SCAT# v4x7# v7x3 V6x3
