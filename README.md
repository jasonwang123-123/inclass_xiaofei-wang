# inclass_xiaofei-wang

import json
with open('cddata','r') as f:
   for line in f:
       try:
          data =json.loads(line)
       exceot:
          data={}
       if 'received' in data.keys():
          if  data['received'] >='2019-01-01' and data['received'] <='2019-01-02':
   
data.append(line)
with open('output.txt', "wb" ) as fp:
  json.dump(data, fp)
       
