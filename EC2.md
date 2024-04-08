### Extend Ubuntu EC2 EBS volume size
```
sudo growpart /dev/nvme0n1 1
sudo resize2fs /dev/nvme0n1p1
```

Mounting efs storage permanently 
```
fs-0fb106bfdc0cc0229.efs.us-east-1.amazonaws.com:/ efs/ nfs4 _netdev 0 0
```

## Copy file from remote server to local mac
```
scp -i /Users/kalindusekarage/AWS-Keys/nodes-key.pem ec2-user@3.91.170.197:"/efs/mnt/content_selection_platform/data/metadata-collector/movies/job_1711572710/A Aa Hindi Dubbed Full Movie New  Nithiin Samantha Anupama Parameshwaran  Trivikram.mp4" ./
```
