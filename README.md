I top5         = ciiScores.slice(0, STRATEGIC_RISK_TOP_N)            # N = 5
weights      = [1.00, 0.85, 0.70, 0.55, 0.40]                       # 1 - i * 0.15
weightedAvg  = Σ(score_i * weight_i) / Σ(weight_i)
overallScore = min(100, round(weightedAvg * 0.70 + 15))             # banded to [15, 85]# World Monitor APP