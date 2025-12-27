# Contribution Guidelines

Welcome to the Arabidopsis thaliana Chromosome 4 gene annotation curation project!

## Workflow

1. **Select a gene**: Pick an unassigned issue titled "Investigate Gene: AT4GXXXXX".
2. **Assign yourself**: Assign the issue to yourself to indicate you are working on it.
3. **Validate the gene model**:
   - Extract the coding sequence from the genomic FASTA using coordinates in the GFF3 file.
   - Perform BLAST search against NCBI nr database to identify homologs.
   - Run ab initio gene prediction (e.g., GeneMark) on the genomic region.
   - Compare predictions to the existing annotation.
4. **Document findings**: Create a validation report in `validation_reports/AT4GXXXXX_validation_report.md`.
5. **Propose corrections**: If needed, edit `chr4_annotation.gff3` to fix errors.
6. **Submit changes**:
   - Commit your changes to a new branch named `curate/AT4GXXXXX`.
   - Open a pull request from your branch to the `main` branch.
   - Link the issue in the PR description (e.g., "Resolves #X").

## Notes

- Ensure your changes follow GFF3 format specifications.
- Provide clear justification for any modifications.
- If the annotation is correct, still submit the validation report without GFF3 changes.

Thank you for contributing!