# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Fixed-effects OLS estimation Use feols (fixest) With (In) R Software
install.packages("fixest")
library("fixest")
feols = read.csv("https://raw.githubusercontent.com/timbulwidodostp/feols/main/feols/feols.csv",sep = ";")
# Estimation Fixed-effects OLS estimation Use feols (fixest) With (In) R Software
Fixed_effects_OLS_estimation = feols(Euros ~  Origin + Destination + Product + Year, feols)
summary(Fixed_effects_OLS_estimation)
Fixed_effects_OLS_estimation_1 = feols(Euros ~  Origin + Destination + Product | Year, feols)
summary(Fixed_effects_OLS_estimation_1)
Fixed_effects_OLS_estimation_2 = fepois(Euros ~ log(dist_km) | Origin + Destination + Product + Year, feols)
summary(Fixed_effects_OLS_estimation_2)
# Fixed-effects OLS estimation Use feols (fixest) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished