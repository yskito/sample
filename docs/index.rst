.. test documentation master file, created by
   sphinx-quickstart on Sun Feb 27 16:35:16 2022.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.

こちらはサンプルページです
================================

.. .. toctree::
   :maxdepth: 2
   :caption: Contents:

================================
folder structure
================================
.. blockdiag::

   blockdiag {

     #===========================
     # folders config
     #===========================
     folder [height = 80]; 
     01_data [height = 80]; 
     02_results [height = 80]; 
     03_fig [height = 80]; 

     #===========================
     # files strucuture
     #===========================
     main.py [shape = note];
     data.csv [shape = note];
     results1.csv [shape = note];
     
     results2.csv [shape = note];
     
     fig1_heatmap.tiff [shape = note];
     
     fig2_plot1.tiff [shape = note];
     
     fig3_plot2.tiff [shape = note];
     
     
     #===========================
     # folder strucuture
     #===========================
     folder -- main.py;
     folder -- 01_data;
          01_data -- data.csv;
     folder -- 02_results;
          02_results -- results1.csv;
          02_results -- results2.csv;
     folder -- 03_fig;
          03_fig -- fig1_heatmap.tiff;
          03_fig -- fig2_plot1.tiff;
          03_fig -- fig3_plot2.tiff;
   }

.. Indices and tables
 ==================

 * :ref:`genindex`
 * :ref:`modindex`
 * :ref:`search`
