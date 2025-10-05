# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Nakagawa's R-squared statistic for multilevel mixed-effects linear regression Use r2_nakagawa (performance) With (In) R Software
install.packages("performance")
install.packages("lme4")
library("performance")
library("lme4")
r2_nakagawa_r = read.csv("https://raw.githubusercontent.com/timbulwidodostp/r2_nakagawa_r/main/r2_nakagawa_r/r2_nakagawa_r.csv",sep = ";")
# Estimation Nakagawa's R-squared statistic for multilevel mixed-effects linear regression Use r2_nakagawa (performance) With (In) R Software
model <- lme4::lmer(Sepal.Length ~ Petal.Length + (1 | Species), data = r2_nakagawa_r)
r2_nakagawa <- r2_nakagawa(model)
r2_nakagawa
r2_nakagawa_group <- r2_nakagawa(model, by_group = TRUE)
r2_nakagawa_group
# Nakagawa's R-squared statistic for multilevel mixed-effects linear regression Use r2_nakagawa (performance) With (In) R Software
# Olah Data Semarang
# WhatsApp : +6285227746673
# IG : @olahdatasemarang_
# Finished