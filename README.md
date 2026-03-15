# Bernoulli Coin Toss Simulator

This Streamlit application provides an interactive visualization of the **Law of Large Numbers** through a simulated Bernoulli trial (coin toss). Users can observe how the cumulative mean of "heads" (successes) converges toward the theoretical probability as the number of iterations increases.

---

## 🚀 Features

* **Real-time Visualization:** Uses an interactive line chart to map the evolving mean as each "coin toss" is processed.


* **Customizable Trials:** A slider allows users to define the number of attempts, ranging from **1 to 1000**.


* **Experiment History:** The app maintains a session state to track results across multiple runs, displaying a summary table of previous experiments.


* **Stochastic Simulation:** Utilizes `scipy.stats.bernoulli` to generate random outcomes based on a probability of $p=0.5$.



---

## 🛠️ Installation

Ensure you have Python installed, then set up the environment using the provided `requirements.txt`.

### 1. Install Dependencies

```bash
pip install -r requirements.txt

```

The core dependencies include **pandas**, **scipy**, and **streamlit**.

### 2. Run the App

```bash
streamlit run app.py

```

---

## 📊 How It Works

1. **Input:** Select the desired number of trials using the sidebar slider.


2. **Execution:** Click **"Ejecutar"** to start the simulation.


3. **Simulation Loop:** * The app generates a sequence of random outcomes.


* It calculates the running mean: $$\bar{x} = \frac{\sum successes}{n}$$.


* The chart updates every **0.05 seconds** to animate the convergence.




4. **Data Logging:** Once complete, the final mean and trial count are appended to the results dataframe stored in the session state.



---

## 📁 File Structure

* `app.py`: The main Python script containing the Streamlit UI and simulation logic.


* `requirements.txt`: List of necessary libraries to run the application.


## ✒️ Autor

* **Luis Ahumada Sánchez** - [Github](https://www.google.com/search?q=https://github.com/luis-ahumadas)

---