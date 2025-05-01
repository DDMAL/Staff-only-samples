# Staff-only-samples

This repo contains (hopefully) all the resources needed to test the `Miyao Staff Finding` job, or any other job that also finds staff lines. Here’s what you need to know:
- `Miyao` is currently working very well for some manuscripts, and very poorly for other manuscripts. 
- Some manuscripts have four-line staves, and some have five-line staves; `Miyao` always works for four-line staves but doesn’t always work for five-line staves. 
- `Miyao` reliably finds staves in the following manuscripts:
  - Salzinnes (4 lines per staff)
  - Einsiedeln (4 lines per staff)
  - MS73 (4 lines per staff)
  - Martha’s manuscript (5 lines per staff)

- `Miyao` finds few to no staves in the following manuscripts:
  - Bach B-minor mass (5 lines per staff)
  - Bach’s well-tempered Clavier (5 lines per staff)
  - Bach Chorales (5 lines per staff)

The `Miyao` job uses the extracted staff line layer of a folio to find the staves. The Rodan workflow that connects the staff line layer to `Miyao` looks like this:

<img width="200" alt="Miyao no fast" src="https://github.com/user-attachments/assets/8e08de39-5269-4372-9321-952d4b75177a" />

And this is the workflow: 
[Staff lines to Miyao workflow.json.zip](https://github.com/user-attachments/files/20006405/Staff.lines.to.Miyao.workflow.json.zip)

This repo contains staff line layers for 5 folios from each of the above manuscripts. For each folio, there is also the output of every intermediary job between the first `PNG` job and `Miyao`. The name of the resource is the job that _output it_. 

There are also two synthetic staff line layers meant to be the control layers. One has a four-line staff, and the other has a five-line staff.

