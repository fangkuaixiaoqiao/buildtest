vendor := $(srctree)/$(src)

#ifndef VENDOR_EDIT
#ifneq "$(wildcard $(vendor)/qcom)" ""
#	subdir-y += qcom
#endif
#else
#	subdir-y += 20031
	subdir-y += qcom
ifeq ($(strip $(CONFIG_CHG_FOR_OP9_PRO)), y)
        subdir-y += oplus/lemonadev
else ifeq ($(strip $(CONFIG_OPLUS_CHG_OP9RT_PMIC_VOOCPHY)), y)
        subdir-y += oplus/martini
else ifeq ($(strip $(OPLUS_VND_BUILD_PLATFORM)), SM7325)
        subdir-y += oplus/walle
        subdir-y += oplus/libai
        subdir-y += oplus/lantian
        subdir-y += oplus/lunaa
        subdir-y += oplus/taylor
        subdir-y += oplus/garbo
        subdir-y += oplus/ziti
else
	subdir-y += oplus/peacock
	subdir-y += oplus/fussi
        subdir-y += oplus/cupid
	subdir-y += oplus/luwu
        subdir-y += oplus/porsche
	subdir-y += oplus/eva
	subdir-y += oplus/fluorite

endif
#endif
