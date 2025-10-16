# Reinforcement-learning-projects
Implementation of Multi-Armed Bandit algorithms — UCB and Thompson Sampling — to explore the balance between exploration and exploitation in reinforcement learning.

This project explores two classic Reinforcement Learning strategies — Upper Confidence Bound (UCB) and Thompson Sampling — to solve the Multi-Armed Bandit problem.
Both algorithms aim to find the best action while balancing exploration (trying new options) and exploitation (using the best-known option).
The project will test and compare their performance using ad selection data to see which method selects the most effective ad.

## UCB
### Formula
<img width="932" height="584" alt="image" src="https://github.com/user-attachments/assets/3344baa9-601c-4558-b5b2-82ffc527714d" />

### Results
When we tested with N = 10,000 (the full dataset), the graph clearly showed that Ad 5 had the highest performance. One key goal of the UCB model is to identify the best possible ad in fewer rounds. So, we also tested with smaller datasets — N = 5,000, N = 1,000, and N = 500. The model still performed well with 5,000 and even 1,000 rounds, successfully selecting Ad 5 as the best. However, with only 500 rounds, the performance dropped, and the model struggled to identify the optimal ad.

### N = 10000
<img width="424" height="268" alt="image" src="https://github.com/user-attachments/assets/d7a843bf-9867-463c-88c5-198645fe9742" />

### N = 5000
<img width="611" height="434" alt="image" src="https://github.com/user-attachments/assets/6aaa5bce-8e74-4c25-972e-121e992f6aa1" />

### N = 1000
<img width="617" height="446" alt="image" src="https://github.com/user-attachments/assets/3172c7ab-a9fc-435d-9f84-9d5dafbcaf53" />

### N = 500
<img width="581" height="450" alt="image" src="https://github.com/user-attachments/assets/83ffdb76-843b-47a7-8e32-48122af5fd73" />

## Thompson Sampling Algorithm
### Formula
<img width="1104" height="469" alt="image" src="https://github.com/user-attachments/assets/a2608c9a-abe4-45c1-89b9-cb76d137da11" />

### Results
When tested Thompson Sampling: For N = 10000, 5000, 1000, and even 500 rounds, it still picked the 5th Ad correctly, just unlike the UCB algorithm where it wasnt able to guess correct AD when N was smaller or 500. That shows Thompson Sampling is more powerful — especially when you have less data (fewer rounds).

