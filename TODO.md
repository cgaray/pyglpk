Change LPX_solver_simplex, LPX_solver_integer to accept new control options.

Tests for...
LPX.erase()
Bar.scale

For each section of the GLPK 4.31 manual that describes functions, this describes the progress in providing the functionality of that procedure in PyGLPK, the corresponding C function, and the source file in which the functionality is provided.

# Version 2
## Version 2.2
*2.2.1  Done, glp_create_prob (lp.c)
*2.2.2  Done, glp_set_prob_name (lp.c)
*2.2.3  Done, glp_set_obj_name (obj.c)
*2.2.4  Done, glp_set_obj_dir (obj.c)
*2.2.5  Done, glp_add_rows (barcol.c)
*2.2.6  Done, glp_add_cols (barcol.c)
*2.2.7  Done, glp_set_row_name (bar.c)
*2.2.8  Done, glp_set_col_name (bar.c)
*2.2.9  Done, glp_set_row_bnds (bar.c)
*2.2.10 Done, glp_set_col_bnds (bar.c)
*2.2.11 Done, glp_set_obj_coef (obj.c)
*2.2.12 Done, glp_set_mat_row (bar.c)
*2.2.13 Done, glp_set_mat_col (bar.c)
*2.2.14 Done, glp_load_matrix (lp.c)
*2.2.15 Done, glp_del_rows (barcol.c)
*2.2.16 Done, glp_del_cols (barcol.c)
*2.2.17 Done, glp_erase_prob (lp.c)
*2.2.18 Done, glp_delete_prob (lp.c)

## Version 2.3
* 2.3.1  Done, glp_get_prob_name (lp.c)
* 2.3.2  Done, glp_get_obj_name (obj.c)
* 2.3.3  Done, glp_get_obj_dir (obj.c)
* 2.3.4  Done, glp_get_num_rows (barcol.c)
* 2.3.5  Done, glp_get_num_cols (barcol.c)
* 2.3.6  Done, glp_get_row_name (bar.c)
* 2.3.7  Done, glp_get_col_name (bar.c)
* 2.3.8  Done, glp_get_row_type (bar.c)
* 2.3.9  Done, glp_get_row_lb (bar.c)
* 2.3.10 Done, glp_get_row_ub (bar.c)
* 2.3.11 Done, glp_get_col_type (bar.c)
* 2.3.12 Done, glp_get_col_lb (bar.c)
* 2.3.13 Done, glp_get_col_ub (bar.c)
* 2.3.14 Done, glp_get_obj_coef (obj.c)
* 2.3.15 Done, glp_get_num_nz (lp.c)
* 2.3.16 Done, glp_get_mat_row (bar.c)
* 2.3.17 Done, glp_get_mat_col (bar.c)
  
* 2.4.1  Done, glp_create_index (barcol.c)
* 2.4.2  Done, glp_find_row (barcol.c)
* 2.4.3  Done, glp_find_col (barcol.c)
* 2.4.4  N/A, glp_delete_index (it is not exactly appropriate anywhere)
  
* 2.5.2  Done, glp_set_rii (bar.c)
* 2.5.3  Done, glp_set_sjj (bar.c)
* 2.5.4  Done, glp_get_rii (bar.c)
* 2.5.5  Done, glp_get_sjj (bar.c)
* 2.5.6  Done, glp_scale_prob (lp.c)
* 2.5.7  Done, glp_unscale_prob (lp.c)
  
* 2.6.2  Done, glp_set_row_stat (bar.c)
* 2.6.3  Done, glp_set_col_stat (bar.c)
* 2.6.4  Done, glp_std_basis (lp.c)
* 2.6.5  Done, glp_adv_basis (lp.c)
* 2.6.6  Done, glp_cpx_basis (lp.c)

## Version 2.7
* 2.7.1  Done, glp_simplex (lp.c)
* 2.7.2  N/A, glp_init_smcp (we don't represent glp_smcp objects explicitly)
* 2.7.3  Done, lpx_exact (lp.c)
* 2.7.4  Done, glp_get_status (lp.c)
* 2.7.5  Done, glp_get_prim_stat (lp.c)
* 2.7.6  Done, glp_get_dual_stat (lp.c)
* 2.7.7  Done, glp_get_obj_val (obj.c)
* 2.7.8  Done, glp_get_row_stat (bar.c)
* 2.7.9  Done, glp_get_row_prim (bar.c)
* 2.7.10 Done, glp_get_row_dual (bar.c)
* 2.7.11 Done, glp_get_col_stat (bar.c)
* 2.7.12 Done, glp_get_col_prim (bar.c)
* 2.7.13 Done, glp_get_col_dual (bar.c)
* 2.7.14 Done, lpx_get_ray_info (lp.c)
* 2.7.15 Done, lpx_check_kkt (lp.c, kkt.c)

## Version 2.8
* 2.8.1  Done, lpx_interior (lp.c)
* 2.8.2  Done, glp_ipt_status (lp.c)
* 2.8.3  Done, glp_ipt_obj_val (lp.c)
* 2.8.4  Done, glp_int_row_prim (bar.c)
* 2.8.5  Done, glp_int_row_dual (bar.c)
* 2.8.6  Done, glp_int_col_prim (bar.c)
* 2.8.7  Done, glp_int_col_dual (bar.c)

## Version 2.9
* 2.9.1  Done, glp_set_col_kind (bar.c)
* 2.9.2  Done, glp_get_col_kind (bar.c)
* 2.9.3  Done, glp_get_num_int (lp.c)
* 2.9.4  Done, glp_get_num_bin (lp.c)
* 2.9.5  Done, glp_intopt (lp.c)
* 2.9.6  N/A, glp_init_iocp (we don't represent glp_iocp objects explicitly)
* 2.9.7  Done, lpx_intopt (lp.c)
* 2.9.8  Done, glp_mip_status (lp.c)
* 2.9.9  Done, glp_mip_obj_val (obj.c)
* 2.9.10 Done, glp_mip_row_val (bar.c)
* 2.9.11 Done, glp_mip_col_val (bar.c)

# Version 3
Changed a couple of the data reading and writing techniques, but frankly I don't care enough about reading problems from datafiles to stop relying upon the compatibility layer.

# Version 4
## Version 4.2
* 4.1 All of this does not appear anywhere within PyGLPK.  My feeling is that few will care about explicitly performing the steps of the simplex algorithm.

* 4.2.3  Done, glp_ios_reason (tree.c)
* 4.2.4  Done, glp_ios_get_prob (tree.c)
* 4.2.5  Done, glp_ios_tree_size (tree.c)
* 4.2.6  Done, glp_ios_curr_node (tree.c)
* 4 .2.7  Done, glp_ios_next_node (tree.c)
* 4.2.8  Done, glp_ios_prev_node (tree.c)
* 4.2.9  Done, glp_ios_up_node (tree.c)
* 4.2.10 Done, glp_ios_node_level (tree.c)
* 4.2.11 Done, glp_ios_node_bound (tree.c)
* 4.2.12 Done, glp_ios_best_node (tree.c)
* 4.2.13 Done, glp_ios_mip_gap (tree.c)
* 4.2.14 N/A, glp_ios_node_data (unfortunately GLPK provides no facilities for determining that the corresponding node has been deallocated -- one would think this would be *absolutely necessary* since one may wish to store data of varying sizes for each node rather than just a single static block, but heck, what do I know...)
* 4.2.15 Done, glp_ios_select_node (tree.c)
* 4.2.16 Done, glp_ios_heur_sol (tree.c)
* 4.2.19 Done, glp_ios_terminate (tree.c)

## Version 4.3
* 4.3.1 N/A, no need to explicitly represent the GLPK long numbers
* 4.3.2 N/A, glp_version (already have glpk.version)
* 4.3.3 Done, glp_term_out (environment.c)
* 4.3.4 Done, glp_term_hook (environment.c)
* 4.3.5 Done, glp_mem_usage (environment.c)
* 4.3.6 Done, glp_mem_limit (environment.c)
* 4.3.7 N/A, glp_free_env (environment.c)

# Version 5
## Version 5.1
* 5.1.1 Update to post glpk-4.47 api.  Remove support for glpk versions before 4.47 for cleaner code.

I'm currently seeing the following errors on trying to compile the module:

> src/environment.c:75:18: error: unknown type name ‘glp_long’
> #define GLP_LONG glp_long
>                  ^
>src/environment.c:80:26: note: in expansion of macro ‘GLP_LONG’
> static PyObject* long2py(GLP_LONG l) {
>                          ^
>src/environment.c: In function ‘Environment_getbytes’:
>src/environment.c:75:18: error: unknown type name ‘glp_long’
> #define GLP_LONG glp_long
>                  ^
>src/environment.c:90:3: note: in expansion of macro ‘GLP_LONG’
>   GLP_LONG b;
>   ^
>src/environment.c:91:3: warning: passing argument 3 of ‘glp_mem_usage’ from incompatible pointer type [enabled by default]
>   glp_mem_usage(NULL, NULL, &b, NULL);
>   ^
>In file included from src/environment.h:24:0,
>                 from src/environment.c:20:
>/usr/local/include/glpk.h:823:6: note: expected ‘size_t *’ but argument is of type ‘int *’
> void glp_mem_usage(int *count, int *cpeak, size_t *total,
>      ^
>src/environment.c:92:3: warning: implicit declaration of function ‘long2py’ [-Wimplicit-function-declaration]
>   return long2py(b);
>   ^
>src/environment.c:92:3: warning: return makes pointer from integer without a cast [enabled by default]
>src/environment.c: In function ‘Environment_getbytes_peak’:
>src/environment.c:75:18: error: unknown type name ‘glp_long’
> #define GLP_LONG glp_long
>                  ^
>src/environment.c:97:3: note: in expansion of macro ‘GLP_LONG’
>   GLP_LONG b;
>   ^
>src/environment.c:98:3: warning: passing argument 4 of ‘glp_mem_usage’ from incompatible pointer type [enabled by default]
>   glp_mem_usage(NULL, NULL, NULL, &b);
>   ^
>In file included from src/environment.h:24:0,
>                 from src/environment.c:20:
>/usr/local/include/glpk.h:823:6: note: expected ‘size_t *’ but argument is of type ‘int *’
> void glp_mem_usage(int *count, int *cpeak, size_t *total,
>      ^
>src/environment.c:99:3: warning: return makes pointer from integer without a cast [enabled by default]
>   return long2py(b);
>   ^
>error: command 'x86_64-linux-gnu-gcc' failed with exit status 1
>make: *** [all] Error 1

These errors appear to be caused by a change in the API in glpk-4.48.  The changelog for 4.48 reads says

> * glpk.h
>   glp_prob declaration changed (now it is incomplete struct);
>   glp_tree declaration changed (now it is incomplete struct);
>   glp_tran declaration changed (now it is incomplete struct);
>   glp_long declaration removed;
>   glp_time declaration removed;
>   glp_difftime removed from API;
>   glp_data removed from API;
>   glp_sdf_* removed from API;
>   glp_mem_usage declaration changed (glp_long -> size_t);
>   glp_realloc declaration added (not documented yet).

1) change glp_mem_usage to use size_t rather than glp_long and return with PyLong_FromSize_t
