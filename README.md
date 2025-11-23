🧩 Jenkins Master–Slave (Agent) Architecture – DevOps Learning

Today I learned how Jenkins uses a Master–Agent (Slave) setup to run builds efficiently in real DevOps environments.

🔹 What is Jenkins Master?

The Jenkins Master is the main server that:

Manages all pipelines

Schedules jobs

Sends tasks to agents

Provides the Jenkins UI

🔹 What are Jenkins Slaves / Agents?

Agents are worker nodes connected to the master. They:

Execute the actual build steps

Run shell commands, Maven builds, Docker builds, etc.

Allow scaling your CI/CD workload

🔹 Why do DevOps teams use Agents?

Run parallel builds

Reduce load on the Jenkins master

Use different OS environments (Linux, Windows, EC2, Docker)

High availability and better performance

🔹 What I practiced today:

Created a Jenkins master on EC2

Added a Jenkins agent (SSH method)

Configured labels for the agent

Ran a simple pipeline on the agent using:

agent { label 'dev' }

Verified builds running from the agent machine

🚀 Skills Improved Today:

✔ Understanding Jenkins architecture
✔ How master schedules jobs
✔ How agents execute builds
✔ Using pipeline labels
✔ Real CI/CD environment setup
