
# 🧹 Docker Cleanup Practices

## 1. Remove unused (dangling) images
These are layers that are not tagged and not referenced by any container.

docker image prune

2. Remove all unused images (including non-dangling)

This removes any image not currently used by a container.

docker image prune -a

3. Remove stopped containers

Frees up space from containers that are no longer running.

docker container prune

4. Full system cleanup (CAUTION)

Removes:
	•	All stopped containers
	•	All unused networks
	•	All dangling/unused images
	•	All build cache

docker system prune -a

⚠ Warning:

Use docker system prune -a only when you’re absolutely sure. It will remove a lot of data and is not reversible.

---
