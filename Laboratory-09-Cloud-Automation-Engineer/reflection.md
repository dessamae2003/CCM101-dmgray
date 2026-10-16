# Mission 9 Reflection

**1. Why is automation critical when managing hundreds of cloud servers?**
Manual administration does not scale. Doing the same task by hand on hundreds of servers is slow and inconsistent, and every repetition is another chance for human error. A script performs the same steps the same way every time, and scheduling removes the need for anyone to remember to run it.

**2. What are the potential dangers of automation?**
Automation multiplies mistakes as efficiently as it multiplies successes. A destructive typo, such as a wrong path in a delete command, scheduled on 1,000 servers could wipe data everywhere before anyone notices. Scripts should be tested on a small group first, reviewed, version controlled, and backed by recoverable backups.

**3. How did writing a Bash script differ from creating a Docker Compose YAML file (Mission 6)?**
Bash is imperative: I wrote the exact steps in order. Docker Compose is declarative: I described the desired state, and Docker worked out how to reach it. Bash gave more control but needed care with order and syntax, while Compose felt more structured and readable.

**4. How has your understanding of Cloud Computing transformed over the course of this semester?**
At the start, cloud computing felt like an abstract term for "someone else's computer." Looking through Laboratories 1 to 9, I now see it as a set of practical skills: designing infrastructure, running containers, managing data, monitoring, securing, and automating. My repository shows that growth from definitions to hands-on work.

**5. Which role did you enjoy the most and why?**
I enjoyed the Cloud Security Engineer role the most because the results were immediate and visible: a single firewall rule changed whether a request succeeded or failed. It made ideas like least privilege and default deny concrete instead of theoretical.
