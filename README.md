## Martian Crater Exploration: Greedy Search vs. Simulated Annealing

---

### Overview

This Python program simulates the exploration of Martian craters using two different search algorithms: Greedy Search and Simulated Annealing. The objective is to determine the effectiveness of each algorithm in guiding an explorer rover to the bottom of a crater, where valuable scientific discoveries may await. By analyzing the performance of these algorithms, engineers can make informed decisions about rover navigation strategies for future Mars exploration missions.

### Introduction

Exploring Martian craters presents a unique challenge due to the potential presence of water and other elements that could provide insights into the planet's geological history and potential habitability. The program aims to evaluate the capabilities of two search algorithms in guiding a rover safely to the bottom of a crater. The Greedy Search algorithm selects the next move based on immediate neighboring pixels, while Simulated Annealing explores a wider range of possibilities, occasionally accepting suboptimal moves to potentially discover deeper regions within the crater.

---

### Problem 1: Greedy Search

**Algorithm Description**

The Greedy Search algorithm selects the neighboring pixel with the lowest depth that satisfies the height difference constraint of 2.0 meters. It iteratively navigates the rover towards the deepest point in the crater, prioritizing immediate gains without considering long-term exploration strategies.

**Results and Analysis**

Greedy Search demonstrates limited effectiveness in reaching the bottom of the crater within the specified iteration limit. Despite its simplicity, the algorithm struggles to find optimal paths, often getting trapped in local minima. The rover's capability to descend into the crater is hindered by the algorithm's myopic decision-making process.

---

### Problem 2: Simulated Annealing

**Algorithm Description**

Simulated Annealing employs a probabilistic approach to exploration, allowing the rover to occasionally accept moves that are not immediately beneficial. This flexibility enables the algorithm to explore diverse paths and potentially discover deeper regions within the crater. By simulating the annealing process, the algorithm gradually explores the search space while balancing exploration and exploitation.

**Results and Analysis**

Simulated Annealing outperforms Greedy Search in reaching deeper regions of the crater. By incorporating probabilistic acceptance of less favorable moves, the algorithm demonstrates better adaptability and effectiveness in navigating challenging terrain conditions. Simulated Annealing offers a robust and flexible approach to crater exploration, making it a recommended choice for rover engineers.

---

### Dependencies:
- Python 3.x
- numpy: For numerical operations and array manipulation.
- skimage: Used for downsampling the height map to improve computational efficiency.
- matplotlib: Enables visualization of the Martian surface and navigation paths.
- plotly: Utilized for creating interactive 3D visualizations of the surface.

**Resources:**
- [mars_map.IMG](https://drive.google.com/file/d/1IJ5QRZ8NcWQh8LFT-xcZuNLNIPtkbB7a/view?usp=share_link) (topographic information of the Martian landscape extracted from HiRISE)
- mars_2D.png (example image for the introduction of the project)
- mars_3D.png (example image for the introduction of the project)

**Note:** Ensure that the HiRISE topography of Mars (mars_map.IMG) is accessible in the program directory for proper functioning.

---

### Conclusion

In conclusion, Simulated Annealing emerges as the preferred algorithm for guiding rover exploration in Martian craters. Its ability to adapt to complex terrain conditions and explore diverse paths makes it well-suited for discovering deeper regions within the crater. By leveraging Simulated Annealing, rover engineers can optimize exploration strategies and increase the likelihood of making significant scientific discoveries on Mars.# Martian-Crater-Exploration-Greedy-Search-vs.-Simulated-Annealing
