##########################################################################
# ---------------------------------------------------------------------------------------------------------------------
# This is Matlab, R, and LaTeX code to produce IPCC AR6 WGI Technical Summary 4, Figure 1 (TS.4 Fig1)
# Creator: Robert Kopp, Rutgers University, and Gregory Garner, Rutgers University 
# Contact: robert.kopp@rutgers.edu
# Last updated on: February 2, 2022
# --------------------------------------------------------------------------------------------------------------------
#
# - Code functionality:
#   - PanelA_Timeseries/Plot_GMSL.m: This script produces Panel (a) of the figure, showing global mean sea level rise from 1900-2150
#   - PanelB_warminglevels/runTSwls_1panel.m: This script plots Panel (b) of the figure, showing committed sea level rise by warming level and timescale 
#   - PanelC_milestone/plot_exceedance_year_allsps.r: This script plots Panel (c) of the figure, showing projected timing of sea-level rise milestones *
# - Input data: Input data for each panel is contained within that panel's directory (with subdirectories for different data sources). Full SSP-based sea level projection data used in panels a and c can be downloaded from https://doi.org/10.5281/zenodo.5914710. *
# - Output variables: The code plots the figure as in the report.
#
# ----------------------------------------------------------------------------------------------------
# Information on  the software used
# - Software Version: Matlab R2018a and R 4.1.2
#  ----------------------------------------------------------------------------------------------------
#
#  License: Apache 2.0
#
# ----------------------------------------------------------------------------------------------------
# How to cite:
#
# When citing this code, please include both the code citation and the following citation for the related report component:
#
# Fox-Kemper, B., H. T. Hewitt, C. Xiao, G. Aðalgeirsdóttir, S. S. Drijfhout, T. L. Edwards, N. R. Golledge, M. Hemer, R. E. Kopp, G. Krinner, A. Mix, D. Notz, S. Nowicki, I. S. Nurhati, L. Ruiz, J-B. Sallée, A. B. A. Slangen, Y. Yu, 2021, Ocean, Cryosphere and Sea Level Change. In: Climate Change 2021: The Physical Science Basis. Contribution of Working Group I to the Sixth Assessment Report of the Intergovernmental Panel on Climate Change [Masson-Delmotte, V., P. Zhai, A. Pirani, S. L. Connors, C. Péan, S. Berger, N. Caud, Y. Chen, L. Goldfarb, M. I. Gomis, M. Huang, K. Leitzell, E. Lonnoy, J. B. R. Matthews, T. K. Maycock, T. Waterfield, O. Yelekçi, R. Yu and B. Zhou (eds.)]. Cambridge University Press. In press.
#
# When citing the SSP-based sea-level projections, please also include the following citation:
#
# Garner, G. G., T. Hermans, R. E. Kopp, A. B. A. Slangen, T. L. Edwards, A. Levermann, S. Nowikci, M. D. Palmer, C. Smith, B. Fox-Kemper, H. T. Hewitt, C. Xiao, G. Aðalgeirsdóttir, S. S. Drijfhout, T. L. Edwards, N. R. Golledge, M. Hemer, G. Krinner, A. Mix, D. Notz, S. Nowicki, I. S. Nurhati, L. Ruiz, J-B. Sallée, Y. Yu, L. Hua, T. Palmer, B. Pearson, 2021. IPCC AR6 Global Mean Sea-Level Rise Projections. Version 20210809. https://doi.org/10.5281/zenodo.5914710.
#
########################################################################
Footer
© 2023 GitHub, Inc.
Footer navigation

    Terms
    Privacy
    Security
    Status
    Docs
    Contact GitHub
    Pricin
