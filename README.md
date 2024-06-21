# Interesting Other Stuff

# Environment

Make sure you set up your virtual environment first

```
python3 -m venv .venv
source .venv/bin/activate
pip install -r requirements.txt
```

# Useful scripts

[vanity_npub](./scripts/vanity_npub.py) is an adaptation of [knmukai/nostr_vanity_npub](https://github.com/kdmukai/nostr_vanity_npub) to generate an npub, the nsec. I added the corresponding mnemonic, or seed phrase. (line 68-72)

example usage is:
```
python scripts/vanity_pub.py ad
```
where 'ad' is the vanity prefix.

The resulting output will look like something like this:

```
['ad']
[]
Initialized 2 threads
2024-06-21 16:01:57.962982: Starting

0 | 0.0s | ad | npub1adtendhqyjpjr272wp485r3je5lhft9zquag6np725nc0efpu2ksrdrvf0

        ****************************************************************************
        Private key: nsec1a8eufd2ammz8fmq8gkpgz48cllr297xl0llxank2uj8ydfl9ydnsdmfs60
        ****************************************************************************


        *********************************************************************************
        Private key hex: e9f3c4b55ddec474ec0745828154f8ffc6a2f8df7ffe6ececae48e46a7e52367
        *********************************************************************************

Mnemonic Phrase: try owner coil roof unable denial quote trim little apple dilemma zebra health ladder law zone human iron rice broken heavy verb mirror trouble
```

