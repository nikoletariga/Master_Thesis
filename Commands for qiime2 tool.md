```markdown
Alternatively in command line you can run the following commands for QIIME 2 tool

## qiime2 tools import

```bash
qiime tools import \
  --type EMPSingleEndSequences \
  --input-path emp-single-end-sequences \
  --output-path emp-single-end-sequences.qza
```

## qiime2 demux summarize

```bash
qiime demux summarize \
  --i-data demux.qza \
  --o-visualization demux.qzv
```

```bash
qiime tools view demux.qzv
```

## qiime2 dada2 denoise-single

```bash
qiime dada2 denoise-single \
  --i-demultiplexed-seqs demux.qza \
  --p-trim-left (number)\
  --p-trunc-len (number)\
  --o-representative-sequences rep-seqs-dada2.qza \
  --o-table table-dada2.qza \
  --o-denoising-stats stats-dada2.qza
```

```bash
qiime metadata tabulate \
  --m-input-file stats-dada2.qza \
  --o-visualization stats-dada2.qzv
```

## qiime2 feature-table summarize & qiime2 feature-table tabulate-seqs

```bash
qiime feature-table summarize \
  --i-table table.qza \
  --o-visualization table.qzv \
  --m-sample-metadata-file sample-metadata.tsv
```

```bash
qiime feature-table tabulate-seqs \
  --i-data rep-seqs.qza \
  --o-visualization rep-seqs.qzv
```
