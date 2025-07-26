### Contributors
	Ushasri Mavuri (ushasri.mavuri@thoughtworks.com)
	Geetha Peddinni (geetha.peddinni@thoughtworks.com)

### Path to Yaml Files
```
	final_assignment/crud_app/
	
	backend-deployement.yaml
	backend-service.yaml
	db-password-secret.yaml
	persistent-volume.yaml
	persistent-volumeclaim.yaml
	postgress-deployment.yaml
	postgress-service.yaml
```
### Namespace Creation

```
 	kubectl create namespace crud-app
 	kubectl config set-context $(kubectl config current-context) --namespace=crud-app
  	kubectl create -f db-password-secret.yaml -n crud-app
  	kubectl create -f postgress-service.yaml -n crud-app
	kubectl create -f postgress-deployment.yaml -n crud-app
  	kubectl create -f backend-service.yaml -n crud-app
 	kubectl create -f backend-deployment.yaml -n crud-app
	kubectl create -f persistent-volume.yaml -n crud-app
	kubectl create -f persistent-volumeclaim.yaml -n crud-app
```

# The Rise of the Containers (semi-guided) material


ROTC is a 2-day hands-on, semi-guided workshop, with an additional four-hour ROTC assignment, where participants will explore Kubernetes and go deeper into its various components. This repository contains learning material for the workshop.


[Final Assignment](https://github.com/twlabs/ROTC-semi-guided-material/tree/main/final_assignment)

## Additional Resources


* [Tips to Navigate Vim](https://github.com/twlabs/ROTC-semi-guided-material/blob/main/vim_tips.md)
* [Docker Cheat sheet](https://docs.google.com/presentation/d/14vYdLjjgNT4Z5R1bpG7s30hziFbPI83nQfhEjueKPjY/edit?usp=sharing)
* [Kubernetes cheat sheet](https://docs.google.com/presentation/d/13eUDCCs7ONLY1cFyUaGERBlgSxtNsYpzi8PwolML_kY/edit#slide=id.g29bb06bcdbf_0_164)
* [Rancher setup guide](https://docs.google.com/document/d/1aWsFkANawEG_LHe1-zKB7e3UERtS53sdUX1h_qnH9uE/edit?usp=sharing)
