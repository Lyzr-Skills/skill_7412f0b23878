# Analysis Contract

All files and pipeline modules must comply with the following structural invariants:

1. **Input Completeness**
   - The analysis MUST include at least Company Name, Geography, and Price Point before executing Stage 2.
2. **Referential Integrity**
   - Every claim in the Persona, Segment, or ICP output must reference one or more valid Evidence IDs (`EV-xxx`) or Signal IDs (`SIG-xxx`).
3. **No Unbacked Persona Attributes**
   - Demographic properties (e.g. age range, preferences) cannot be synthesized from general marketing personas. If evidence does not exist, status fields must reflect `unknown`.
4. **Mutually Exclusive Roles**
   - ICP definition models the *organization*. Persona models the *human*. They cannot be nested as single flat records.
