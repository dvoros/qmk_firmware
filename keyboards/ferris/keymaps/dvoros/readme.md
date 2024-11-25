# README

- Need to edit `keymap.c` to make changes.
- This configurator can come in handy, use it to create something and then export to JSON. Then turn JSON into c with `qmk json2c`. Copy the parts you need to your `keymap.c`.
- Flash to keyboard with:

```bash
# Test compilation:
qmk compile -kb ferris/sweep -km dvoros

# Test the two halves separately:
make CONVERT_TO=promicro_rp2040 ferris/sweep:dvoros:uf2-split-right
make CONVERT_TO=promicro_rp2040 ferris/sweep:dvoros:uf2-split-left
```

