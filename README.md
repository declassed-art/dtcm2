# Declassed Tor Circuits Manager version 2

This is a mirror of the [main repository](https://declassed.art/repository/dtcm2).

Maintain the specified number of circuits and attach streams to them in a round-robin manner.

How to use:

```python

    from dtcm2 import TorCircuitsManager

    async with TorCircuitsManager('127.0.0.1', 9051, 'my-secret-password',
                                  hops=2, num_circuits=500) as tcm:
        await tcm.run()
```

Mind exceptions and re-run this block when shit happens. Up to you.

This module uses [torcontrol](https://github.com/declassed-art/torcontrol).
See also Stem-based version 1: https://declassed.art/repository/dtcm
