# MotorAI_assignment2_b

Some features share the same values in one or two channels this can create confusion for ML pipelines. When it tries to interpret the RGB triplets as integers or categories but gets multiple values mapping to similar-looking pixels.Most ML models expect each class label to be a single integer value, not an RGB triplet. Feeding a full-color RGB mask without mapping it to class IDs likely caused:
Culprits: Road markings like solid line and dashed line, which had similar green values, were likely the problem.
Solution: Instead of an RGB pixel values, use a single-band raster with unique integer class IDs. This ensures clear, distinct labels for training ML models.
