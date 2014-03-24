key2bag
=======

##Installation

####Installing into system bin
```
git clone git@github.com:adamenger/key2bag.git
sudo ln -s key2bag/key2bag /usr/local/bin/key2bag
```

####Creating custom bin directory and adding it to your path
```
mkdir ~/bin
cp key2bag/key2bag ~/bin/key2bag
echo "export PATH=~/bin:$PATH" >> ~/.bash_profile"
source ~/.bash_profile
```

## Usage

Try generating a test key [here](http://travistidwell.com/jsencrypt/demo/) and saving it to key.txt.

Then you should be able to 

```
$cat key.txt | key2bag

-----BEGIN RSA PRIVATE KEY-----\nMIICWwIBAAKBgG5L+LAkqZnI2qyXCcPcUMhErTifaI6g5t36datgShzUsFUpXQ09\nDRvFoxVdewfpKRKu3co/pCQ7aoMXuPo5L/E2D6p1cuenDwlhCnZ/F1Dpjrf3emNS\nyWwBoTc1xJ3pVy5+fyuhBeOHJM1kjp9QtLBsPhtUXPOXhlvIauMkvqAjAgMBAAEC\ngYBV438i20ne4VO3tl36USPu79vcDfZDqvRcw17CN1c/IDi3+F/noTUF/V9Dkenu\nfRho3hcEGY7eUA5fSyfWYpX7wCBNbKMSVvcmHNdMHCVAOTtHfdFNGbOInWhrlt0y\n9ysVQ19KmwkDtxKRHra7n5yYddqZBO5K9LP/v9bDL6aYkQJBAKmUVKRszMn3AbOy\nGEaGn/3cHe1oyribiwW3SDjpaunRjo8hDk8Iycb6bGFaevKxUZJEWHKUfm8ArWxF\n6JH1QS0CQQCmgYHqLtUEWozed6ecl7tpjFWC/J+euIRJ7nu6RDNTzhPWqi5nbhps\nIbW7FKDRqsNLfQXASbJ9/pnS/LkhDxiPAkA6IF3i/mgz0jcDIUiw4/RzT7/yYLkc\nDjTZALoAyAGdo/b5mJsO/DQtwCjmNd1u0tjjCgpHPB8abWEEe/H8FdUBAkEAoQAV\nKOZD38PW9r5oeghVlYe2n8O6bHUqpXpOdRvBLcXUdPt1h1l1fx1RZiZaIqKl2HZ5\neydHyoDHKLZqJEc+jQJAO/nC2tg//U28sSFBlqdE2IHuRo9BmjzrH36tqbufMNSE\nTqzviOB/wpCEJt7OT9yJquYU734W/1/K9QhH7YINOw==\n-----END RSA PRIVATE KEY-----

```

Simply copy the string into your encrypted data bag and voila!
