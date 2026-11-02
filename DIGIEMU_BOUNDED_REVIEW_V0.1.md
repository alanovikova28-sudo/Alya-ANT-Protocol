{
  "schema_version": "1.0",
  "experiment_id": "ANT_ALYOSHA_VSC_001",
  "freeze_date": "2026-09-29",
  "runtime": {
    "runtime_family": "Ollama / Docker",
    "ollama_version": null,
    "execution_environment": "Docker Container Engine, isolated node"
  },
  "model": {
    "tag": "qwen3.6:35b",
    "digest": "096fdbd02fe6",
    "quantization": "INT4"
  },
  "sampling": {
    "temperature": 0.55,
    "seed": 15,
    "additional_parameters": "NOT PROVIDED"
  },
  "context": {
    "configured_window_tokens": 50000,
    "cp09_target_tokens": 45000,
    "cp10_target_tokens": 50000,
    "checkpoint_values_are_approximate_targets": true,
    "actual_measurement_method": "standard Qwen tokenizer"
  },
  "conditions": {
    "control": {
      "ant": "OFF",
      "mechanism": "vanilla Ollama image"
    },
    "treatment": {
      "ant": "ON",
      "mechanism": "ANT latent proxy intercepting logits prior to sampling"
    },
    "fresh_identical_initial_state": true
  },
  "ant": {
    "version_or_build_id": "NOT PROVIDED",
    "telemetry_export": "SEPARATE",
    "telemetry_role": "EXPLORATORY_NON_SCORING"
  }
}
