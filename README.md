# Transcriptional
Heatmap
pheatmap(log2(exprSet+1),
         annotation_col = annotation_col,
         annotation_colors = annColors,
         scale = 'row',
         color = colorRampPalette(c("blue","white","red"))(100),
         cluster_rows  = T,
         cluster_cols = F,
         show_rownames = F,
         show_colnames = F,
         gaps_col = 5,
         legend = T,
         legend_postion="left",
         main = 'DEGs_heatmap'
         )
#移动图片位置
grid.edit("layout", vp = viewport(x = unit(0.5, "npc"), y = unit(0.5, "npc")))
