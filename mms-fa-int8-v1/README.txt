高精度切分模型 / Precise alignment model
MMS forced-alignment model (Meta AI, "Scaling Speech Technology to 1,000+ Languages", Pratap et al., 2023),
as packaged by torchaudio.pipelines.MMS_FA; exported to ONNX and dynamically quantized to int8 by this site
(scripts/audio/export_mms_onnx.py). Waveform normalization and log-softmax are done in the page.
License: Creative Commons Attribution-NonCommercial 4.0 (CC BY-NC 4.0), https://creativecommons.org/licenses/by-nc/4.0/
This site is non-commercial. Changes: converted to ONNX, weights quantized to 8-bit.
Split into parts by scripts/audio/publish-align-models.mjs; see manifest.json (sha256 of the whole file).
