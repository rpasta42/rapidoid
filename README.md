
## Instructions

```bash
sudo su
ansible-playbook sndr.yaml  -i hosts.ans
```

Test URL
http://sndr-oss-rapidoid-challenge-1329829309.us-east-2.elb.amazonaws.com/factors


Check for http/2 (not implemented yet)
```
from hyper import HTTPConnection
c = HTTPConnection('sndr-oss-rapidoid-challenge-1329829309.us-east-2.elb.amazonaws.com')
c.request('GET', '/factors')
resp = c.get_response()
```
