# 👋 Hi, I'm Giacomo Falcone

🎓 MSc in Computer Science & Engineering (FinTech), Politecnico di Milano & Université de Rennes (EIT Digital double degree)  
🔬 Master's thesis at IRISA (Inria / CNRS) on succinct proofs for Bitcoin light clients  
📈 I work where distributed systems meet finance: blockchain protocols, quantitative trading, and machine learning on market data  
🏅 1st place in the Université de Rennes ranking, Bloomberg Global Trading Challenge

## 🔧 Skills

- **Blockchain:** consensus protocols, light clients (NIPoPoWs), Bitcoin internals, L2 scaling, cryptography
- **Finance & Quant:** financial markets, time-series analysis, reinforcement learning for trading, risk-adjusted performance metrics
- **Machine Learning:** Scikit-Learn, PyTorch, TensorFlow, Stable-Baselines3
- **Engineering:** Rust, Python (Pandas, NumPy), Java, SQL · distributed systems, networking (TCP/IP) · Git, Docker, LaTeX

## 🏆 Projects

### 🔹 **Sesterce Explorer: Succinct Proofs on Bitcoin Mainnet**
*Master's thesis · IRISA, PIRAT team (Inria / CNRS)*  
A live Bitcoin explorer that compresses the entire chain (965K blocks) into a variable-difficulty NIPoPoW and keeps it in sync with mainnet as new blocks are mined.
- Retains 1 block in 139 and updates the proof in ~87 ms per block, using only the proof itself after a one-time initial pass
- Byte-level cost model of the proof: 5.3 MB to select the chain, 29.7 MB to validate and mine, vs ~1 TB for a full node
- Concurrent backend over three node channels (LevelDB, JSON-RPC, ZeroMQ) with reorg recovery
- Co-author of a research paper (in preparation) on the security of variable-difficulty NIPoPoWs

📌 *Tech: Rust, Rocket, Bitcoin Core, LevelDB, ZeroMQ*

### 🔹 **Reinforcement Learning for Crypto Trading**
Custom Gymnasium environment simulating crypto trade execution on 3 years of tick data, with a PPO (actor-critic) agent trading long, short and flat over 3M+ timesteps.
- Log-return reward shaping targeting risk-adjusted performance (Sharpe ratio)
- Partial observability addressed by adding portfolio latency and order-book depth to the agent's state
- Positive PnL on unseen ETH data during out-of-sample validation

📌 *Tech: Python, Stable-Baselines3, Gymnasium, Pandas*  
🔗 [View project](https://github.com/giacomofalcone/crypto-rl-trading)

### 🔹 **Crypto Crash Prediction from Alternative Data**
Pipeline from raw Reddit dumps (Pushshift, .zst) to a model predicting crypto market crashes.
- Filtered millions of posts and built 2-hour features combining VADER sentiment with Google Trends
- Random Forest regressor reaching R² of 0.94 on the LUNA crash and 0.74 on the FTX collapse, validated on crisis events unseen in training

📌 *Tech: Python, Pandas, Scikit-Learn, VADER*  
🔗 [View project](https://github.com/giacomofalcone/crypto-sentiment-analysis)

### 🔹 **Deep Learning for Computer Vision**
Two team challenges from the Artificial Neural Networks and Deep Learning course at Politecnico di Milano.
- **Blood cell classification (8 classes):** fine-tuned ConvNeXt with RandAugment and class weighting, 77% test accuracy
- **Mars terrain segmentation (5 classes):** U-Net with squeeze-and-excitation blocks and weighted loss, 73.2% mean IoU
- Ranked 22nd of 197 teams in the course challenge

📌 *Tech: Python, ConvNeXt, U-Net, transfer learning, data augmentation*  
🔗 [View project](https://github.com/giacomofalcone/deep-learning-AN2DL)

### 🔹 **Concurrent Client-Server Game (Codex Naturalis)**
Team project: a multiplayer implementation of the board game on a Java client-server architecture.
- Multiple simultaneous game sessions over TCP sockets, with thread-safe controllers
- MVC design with separate GUI and TUI clients
- 90%+ JUnit test coverage

📌 *Tech: Java, TCP/IP, concurrency, JUnit*  
🔗 [View project](https://github.com/giacomofalcone/ing-sw-2024-dicarlo-falcone-foini-gallo)

## 🌍 Languages
🇮🇹 Italian (native) | 🇬🇧 English (C1) | 🇸🇮 Slovenian (C1) | 🇪🇸 Spanish (B1)

## 📫 Let's connect!
📍 Milan, Italy · open to relocation in Europe  
✉️ **Email:** falconegiacomo45@gmail.com  
🔗 **LinkedIn:** [Giacomo Falcone](https://linkedin.com/in/falcone-giacomo)
