# Steps

```powershell
$project="vacationapp01"
gcloud builds submit --tag gcr.io/${project}/helloworld
gcloud run deploy --image gcr.io/${project}/helloworld --platform managed --region=us-central1 --allow-unauthenticated helloworld
```

Do not forget to delete the service after you are done to avoid being charged
