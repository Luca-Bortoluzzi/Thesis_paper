Thesis revision status (updated 14 Oct 2026)

1. Scalability wording
   - Chapters 7 and 8 distinguish translator scalability, benchmarked in
     Chapter 6 with synthetic inputs of up to 10,000 nodes, from the untested
     runtime scalability of starting and executing laboratories of that size.

2. Controlled-load and mitigation results
   - Chapter 5 reports five complete direct-server executions and five complete
     reverse-proxy executions.
   - Every direct-server baseline completed 80/80 requests. During each complete
     transition run, 16/80 requests completed; all 16 preceded workload
     activation, so active-load availability in rounds 3--10 was 0/64 (0%).
   - Every reverse-proxy baseline and controlled-load phase completed 80/80
     requests; active-load availability was 64/64 (100%) in every run.
   - Claims are limited to the tested topology, bounded connection-oriented
     workload, parameters, host, and acquisition period.

3. Repeated-run analysis
   - The statistical unit is one complete execution rather than an individual
     request. Chapter 5 reports descriptive run-level summaries across five
     paired acquisition blocks.
   - The figure now plots the observed values for all five blocks directly;
     no distribution is fitted to the small sample.

4. Wireshark runtime evidence
   - The runtime screenshot is present as images/wireshark_capture.png and is
     included in Chapter 4.

5. Literature, traceability, and validity additions
   - Chapter 1 now positions the framework explicitly against Mininet,
     Kathara, and LLM-assisted network configuration, including a comparison
     table that distinguishes their scopes and validation boundaries.
   - Chapter 2 contains a traceability matrix linking FR1--FR17 to the
     implementation and verification evidence presented in the thesis.
   - Chapter 5 contains a dedicated threats-to-validity section covering
     construct, internal, external, and conclusion validity.
   - No persistent repository identifier or stable artefact reference has been
     added at this stage.

6. Editorial corrections
   - Inline long command-line options preserve their literal two leading
     hyphens in the compiled PDF.
   - The static-route YAML example in Chapter 6 has valid indentation.
   - Long filenames and bibliography URLs are formatted to avoid text extending
     into the margins.

The PDF should be rebuilt after any further source change and checked for
undefined citations, undefined references, and overfull boxes.
