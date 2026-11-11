![Noam Revivo](assets/banner.png)

# AI engineering & applied machine learning

I’m a Computer Science graduate pursuing an M.Sc. in Machine Learning & Data Science at Reichman University. I build forecasting systems and train models in PyTorch. I’m especially interested in how to tell whether a model is useful, from checking forecast probabilities against real outcomes to testing whether personalized recommendations beat a simple popularity ranking.

[Portfolio](https://noamrevivo.info) · [LinkedIn](https://linkedin.com/in/noam-revivo)

## ANIZAI · Forecasting with cited evidence

Given a question about a future event, ANIZAI estimates its probability and shows the sources, competing signals, and gaps behind the estimate. I built a LangGraph workflow that retrieves research, public discussion, and market indicators in parallel. A separate calibration tool compares forecasts with resolved prediction-market outcomes.

I built the streaming pipeline with Kafka and PyFlink to integrate nine external sources. It processed **36,000+ records in one documented 24-hour run**. I deployed the containerized AI and data services on Google Kubernetes Engine.

[Explore ANIZAI](https://github.com/NRevivo/Anizai) · [See the pipeline architecture](https://github.com/NRevivo/Anizai/blob/main/docs/images/architecture-data-pipeline.png)

## Machine learning projects

**Image reconstruction and generation.** I trained a differentiable triangle renderer in PyTorch, then froze its weights and optimized the triangles’ positions and colors to reconstruct a target image. I also implemented a GAN for handwritten digit generation and a CycleGAN for translation between unpaired image collections.

**Personalized recommendations · in progress.** I’m building a collaborative filtering model from historical user–item interactions. I’m evaluating matrix factorization against a popularity-based baseline using ranking metrics.

## LINKER · Backend engineering in Python

I built a URL shortener with FastAPI and PostgreSQL. When concurrent requests generate the same short code, a database uniqueness constraint catches the collision and the service retries. An in-memory repository lets me test that behavior in isolation with Pytest. Docker Compose runs the API and database together.

[Explore LINKER](https://github.com/NRevivo/linker-project) · [Read the URL service](https://github.com/NRevivo/linker-project/blob/main/python/app/service/url_service.py)
