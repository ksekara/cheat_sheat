### Extend Ubuntu EC2 EBS volume size
'''
sudo growpart /dev/nvme0n1 1
sudo resize2fs /dev/nvme0n1p1
'''

Mounting efs storage permanently 
'''
fs-0fb106bfdc0cc0229.efs.us-east-1.amazonaws.com:/ efs/ nfs4 _netdev 0 0
'''
