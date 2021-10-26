# check-input

For check some inputs when use [`workflow_dispatch` with `inputs`](https://github.blog/changelog/2020-07-06-github-actions-manual-triggers-with-workflow_dispatch/)

## Example

### Check env input

```yaml
- name: Check env input
  uses: actions/check-input@v1
  with:
    inputs: 'dev hom prd'
    input: ${{ github.event.inputs.env }}
    input-name: 'Environment'
```
