
    
<div class="SelectMenu">
  <div class="SelectMenu-modal">
    <header class="SelectMenu-header">
      <span class="SelectMenu-title">Switch branches/tags</span>
      <button class="SelectMenu-closeButton" type="button" data-toggle-for="branch-select-menu"><svg aria-label="Close menu" aria-hidden="false" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg></button>
    </header>

    <input-demux data-action="tab-container-change:input-demux#storeInput tab-container-changed:input-demux#updateInput">
      <tab-container class="d-flex flex-column js-branches-tags-tabs" style="min-height: 0;">
        <div class="SelectMenu-filter">
          <input data-target="input-demux.source"
                 id="context-commitish-filter-field"
                 class="SelectMenu-input form-control"
                 aria-owns="ref-list-branches"
                 data-controls-ref-menu-id="ref-list-branches"
                 autofocus
                 autocomplete="off"
                 aria-label="Find or create a branch…"
                 placeholder="Find or create a branch…"
                 type="text"
          >
        </div>

        <div class="SelectMenu-tabs" role="tablist" data-target="input-demux.control" >
          <button class="SelectMenu-tab" type="button" role="tab" aria-selected="true">Branches</button>
          <button class="SelectMenu-tab" type="button" role="tab">Tags</button>
        </div>

        <div role="tabpanel" id="ref-list-branches" data-filter-placeholder="Find or create a branch…" tabindex="" class="d-flex flex-column flex-auto overflow-auto">
          <ref-selector
            type="branch"
            data-targets="input-demux.sinks"
            data-action="
              input-entered:ref-selector#inputEntered
              tab-selected:ref-selector#tabSelected
              focus-list:ref-selector#focusFirstListMember
            "
            query-endpoint="/estebanpscl/Projet_SVM/refs"
            can-create
            cache-key="v0:1675984900.2224839"
            current-committish="bWFpbg=="
            default-branch="bWFpbg=="
            name-with-owner="ZXN0ZWJhbnBzY2wvUHJvamV0X1NWTQ=="
            prefetch-on-mouseover
          >

            <template data-target="ref-selector.fetchFailedTemplate">
              <div class="SelectMenu-message" data-index="{{ index }}">Could not load branches</div>
            </template>

              <template data-target="ref-selector.noMatchTemplate">
    <create-repo-from-selector
      check-tag-name-exists-path="/estebanpscl/Projet_SVM/branches/check_tag_name_exists"
    >
      <!-- '"` --><!-- </textarea></xmp> --></option></form><form data-turbo="false" action="/estebanpscl/Projet_SVM/branches" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="485lV0DRBi3ToB-5xpFfEgQb6jMQtoYoAov5dGSUg2a3r1TcQLq-AKDLjk6paVkeWDicEZWvmPp1oAp0wfANqg" />
        <input data-target="create-repo-from-selector.refName" type="hidden" name="name" value="{{ refName }}">
        <input type="hidden" name="branch"  value="main">
        <input type="hidden" name="path_binary" value="UkVBRE1FLm1k">

        <button
          class="SelectMenu-item wb-break-word"
          type="submit"
          role="menuitem"
          data-index="{{ index }}"
          data-action="click:create-repo-from-selector#createBranch"
          data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;REFS_SELECTOR_MENU_CREATE_BRANCH&quot;,&quot;repository_id&quot;:599798490,&quot;ref_name&quot;:&quot;{{ refName }}&quot;,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="effcc9f54239d3f364c5d890d6b73fae260466fa5e35bda1e0ac6374fe4af2c3">
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-git-branch SelectMenu-icon flex-self-baseline">
    <path fill-rule="evenodd" d="M11.75 2.5a.75.75 0 100 1.5.75.75 0 000-1.5zm-2.25.75a2.25 2.25 0 113 2.122V6A2.5 2.5 0 0110 8.5H6a1 1 0 00-1 1v1.128a2.251 2.251 0 11-1.5 0V5.372a2.25 2.25 0 111.5 0v1.836A2.492 2.492 0 016 7h4a1 1 0 001-1v-.628A2.25 2.25 0 019.5 3.25zM4.25 12a.75.75 0 100 1.5.75.75 0 000-1.5zM3.5 3.25a.75.75 0 111.5 0 .75.75 0 01-1.5 0z"></path>
</svg>
          <div>
            <span class="text-bold">Create branch: {{ refName }}</span>
            <span class="color-fg-muted">from ‘main’</span>
            <input type="hidden" value="F-yB2jm7uPKyFTQSHXxt4jVnQf5e5O-1uTSYZ7bPRtv_9A2zfFfwW7uS8RpwmDoeo8DjER3_MZjPdd32oSLQmw" data-csrf="true" data-target="create-repo-from-selector.checkTagNameExistsPathCsrf" />
          </div>
        </button>
</form>    </create-repo-from-selector>
</template>


            <div data-target="ref-selector.listContainer" role="menu" class="SelectMenu-list " data-turbo-frame="repo-content-turbo-frame">
              <div class="SelectMenu-loading pt-3 pb-0 overflow-hidden" aria-label="Menu is loading">
                <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="32" height="32" viewBox="0 0 16 16" fill="none" data-view-component="true" class="anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
              </div>
            </div>

              

<template data-target="ref-selector.itemTemplate">
  <a href="https://github.com/estebanpscl/Projet_SVM/blob/{{ urlEncodedRefName }}/README.md" class="SelectMenu-item" role="menuitemradio" rel="nofollow" aria-checked="{{ isCurrent }}" data-index="{{ index }}" >
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check SelectMenu-icon SelectMenu-icon--check">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    <span class="flex-1 css-truncate css-truncate-overflow {{ isFilteringClass }}">{{ refName }}</span>
    <span hidden="{{ isNotDefault }}" class="Label Label--secondary flex-self-start">default</span>
  </a>
</template>


              <footer class="SelectMenu-footer"><a href="/estebanpscl/Projet_SVM/branches">View all branches</a></footer>
          </ref-selector>

        </div>

        <div role="tabpanel" id="tags-menu" data-filter-placeholder="Find a tag" tabindex="" hidden class="d-flex flex-column flex-auto overflow-auto">
          <ref-selector
            type="tag"
            data-action="
              input-entered:ref-selector#inputEntered
              tab-selected:ref-selector#tabSelected
              focus-list:ref-selector#focusFirstListMember
            "
            data-targets="input-demux.sinks"
            query-endpoint="/estebanpscl/Projet_SVM/refs"
            cache-key="v0:1675984900.2224839"
            current-committish="bWFpbg=="
            default-branch="bWFpbg=="
            name-with-owner="ZXN0ZWJhbnBzY2wvUHJvamV0X1NWTQ=="
          >

            <template data-target="ref-selector.fetchFailedTemplate">
              <div class="SelectMenu-message" data-index="{{ index }}">Could not load tags</div>
            </template>

            <template data-target="ref-selector.noMatchTemplate">
              <div class="SelectMenu-message" data-index="{{ index }}">Nothing to show</div>
            </template>

              

<template data-target="ref-selector.itemTemplate">
  <a href="https://github.com/estebanpscl/Projet_SVM/blob/{{ urlEncodedRefName }}/README.md" class="SelectMenu-item" role="menuitemradio" rel="nofollow" aria-checked="{{ isCurrent }}" data-index="{{ index }}" >
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check SelectMenu-icon SelectMenu-icon--check">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    <span class="flex-1 css-truncate css-truncate-overflow {{ isFilteringClass }}">{{ refName }}</span>
    <span hidden="{{ isNotDefault }}" class="Label Label--secondary flex-self-start">default</span>
  </a>
</template>


            <div data-target="ref-selector.listContainer" role="menu" class="SelectMenu-list" data-turbo-frame="repo-content-turbo-frame">
              <div class="SelectMenu-loading pt-3 pb-0 overflow-hidden" aria-label="Menu is loading">
                <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="32" height="32" viewBox="0 0 16 16" fill="none" data-view-component="true" class="anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
              </div>
            </div>
              <footer class="SelectMenu-footer"><a href="/estebanpscl/Projet_SVM/tags">View all tags</a></footer>
          </ref-selector>
        </div>
      </tab-container>
    </input-demux>
  </div>
</div>

  </details>

</div>


<div class="Overlay--hidden Overlay-backdrop--center" data-modal-dialog-overlay>
  <modal-dialog role="dialog" id="warn-tag-match-create-branch-dialog" aria-modal="true" aria-labelledby="warn-tag-match-create-branch-dialog-header" data-view-component="true" class="Overlay Overlay--width-large Overlay--height-auto Overlay--motion-scaleFade">
      <header class="Overlay-header Overlay-header--large Overlay-header--divided">
        <div class="Overlay-headerContentWrap">
          <div class="Overlay-titleWrap">
            <h1 id="warn-tag-match-create-branch-dialog-header" class="Overlay-title">Name already in use</h1>
          </div>
          <div class="Overlay-actionWrap">
            <button data-close-dialog-id="warn-tag-match-create-branch-dialog" aria-label="Close" type="button" data-view-component="true" class="close-button Overlay-closeButton"><svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg></button>
          </div>
        </div>
      </header>
    <div class="Overlay-body ">
      
          <div data-view-component="true">      A tag already exists with the provided branch name. Many Git commands accept both tag and branch names, so creating this branch may cause unexpected behavior. Are you sure you want to create this branch?
</div>

    </div>
      <footer class="Overlay-footer Overlay-footer--alignEnd">
            <button data-close-dialog-id="warn-tag-match-create-branch-dialog" type="button" data-view-component="true" class="btn">    Cancel
</button>
            <button data-submit-dialog-id="warn-tag-match-create-branch-dialog" type="button" data-view-component="true" class="btn-danger btn">    Create
</button>
      </footer>
</modal-dialog></div>


  <h2 id="blob-path" class="breadcrumb flex-auto flex-self-center min-width-0 text-normal mx-2 width-full width-md-auto flex-order-1 flex-md-order-none mt-3 mt-md-0">
    <span class="js-repo-root text-bold"><span class="js-path-segment d-inline-block wb-break-all"><a data-turbo-frame="repo-content-turbo-frame" href="/estebanpscl/Projet_SVM"><span>Projet_SVM</span></a></span></span><span class="separator">/</span><strong class="final-path">README.md</strong>
  </h2>
    <a href="/estebanpscl/Projet_SVM/find/main" data-pjax="" data-hotkey="t" data-view-component="true" class="btn mr-2 d-none d-md-block">    Go to file
</a>
  <details id="blob-more-options-details" data-view-component="true" class="details-overlay details-reset position-relative">
    <summary role="button" data-view-component="true" class="btn">    <svg aria-label="More options" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-kebab-horizontal">
    <path d="M8 9a1.5 1.5 0 100-3 1.5 1.5 0 000 3zM1.5 9a1.5 1.5 0 100-3 1.5 1.5 0 000 3zm13 0a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path>
</svg>
</summary>
  <div data-view-component="true">      <ul class="dropdown-menu dropdown-menu-sw">
        <li class="d-block d-md-none">
          <a class="dropdown-item d-flex flex-items-baseline" data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;FIND_FILE_BUTTON&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="107d3dea89846c60ef1c0b987a2e1410201d8188d0272bc14e077f30fab1813e" data-ga-click="Repository, find file, location:repo overview" data-hotkey="t" href="/estebanpscl/Projet_SVM/find/main">
            <span class="flex-auto">Go to file</span>
            <span class="text-small color-fg-muted" aria-hidden="true">T</span>
</a>        </li>
        <li data-toggle-for="blob-more-options-details">
            <button data-toggle-for="jumpto-line-details-dialog" type="button" data-view-component="true" class="dropdown-item btn-link">    <span class="d-flex flex-items-baseline">
              <span class="flex-auto">Go to line</span>
              <span class="text-small color-fg-muted" aria-hidden="true">L</span>
            </span>
</button>        </li>
        <li class="dropdown-divider" role="none"></li>
        <li>
          <clipboard-copy data-toggle-for="blob-more-options-details" aria-label="Copy path" value="README.md" data-view-component="true" class="dropdown-item cursor-pointer">
    
            Copy path

</clipboard-copy>        </li>
        <li>
          <clipboard-copy data-toggle-for="blob-more-options-details" aria-label="Copy permalink" value="https://github.com/estebanpscl/Projet_SVM/blob/550d1a20fd36ecc539338565408de5c95fb68d16/README.md" data-view-component="true" class="dropdown-item cursor-pointer">
    
            <span class="d-flex flex-items-baseline">
              <span class="flex-auto">Copy permalink</span>
            </span>

</clipboard-copy>        </li>
      </ul>
</div>
</details></div>





    <div id="spoof-warning" class="mt-0 pb-3" hidden aria-hidden>
  <div data-view-component="true" class="flash flash-warn mt-0 clearfix">
  
  
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert float-left mt-1">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>

      <div class="overflow-hidden">This commit does not belong to any branch on this repository, and may belong to a fork outside of the repository.</div>


  
</div></div>

    <include-fragment src="/estebanpscl/Projet_SVM/spoofed_commit_check/550d1a20fd36ecc539338565408de5c95fb68d16" data-test-selector="spoofed-commit-check"></include-fragment>

    <div class="Box d-flex flex-column flex-shrink-0 mb-3">
  <include-fragment src="/estebanpscl/Projet_SVM/contributors/main/README.md" class="commit-loader">
    <div class="Box-header d-flex flex-items-center">
      <div class="Skeleton avatar avatar-user flex-shrink-0 ml-n1 mr-n1 mt-n1 mb-n1" style="width:24px;height:24px;"></div>
      <div class="Skeleton Skeleton--text col-5 ml-2">&nbsp;</div>
    </div>

    <div class="Box-body d-flex flex-items-center" >
      <div class="Skeleton Skeleton--text col-1">&nbsp;</div>
      <span class="color-fg-danger h6 loader-error">Cannot retrieve contributors at this time</span>
    </div>
</include-fragment></div>



      








    <readme-toc>

    <div data-target="readme-toc.content" class="Box mt-3 position-relative">
      
  <div
    class="Box-header js-blob-header blob-header js-sticky js-position-sticky top-0 p-2 d-flex flex-shrink-0 flex-md-row flex-items-center"
    style="position: sticky; z-index: 1;"
  >

      <details
  data-target="readme-toc.trigger"
  data-menu-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;trigger&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}"
  data-menu-hydro-click-hmac="a56e58edc6afea0e41798d3193fe14f061f5d2f4dbe3d7be5b1c75e92aeef5d5"
  class="dropdown details-reset details-overlay"
>
  <summary
    class="btn btn-octicon m-0 mr-2 p-2"
    aria-haspopup="true"
    aria-label="Table of Contents">
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-list-unordered">
    <path fill-rule="evenodd" d="M2 4a1 1 0 100-2 1 1 0 000 2zm3.75-1.5a.75.75 0 000 1.5h8.5a.75.75 0 000-1.5h-8.5zm0 5a.75.75 0 000 1.5h8.5a.75.75 0 000-1.5h-8.5zm0 5a.75.75 0 000 1.5h8.5a.75.75 0 000-1.5h-8.5zM3 8a1 1 0 11-2 0 1 1 0 012 0zm-1 6a1 1 0 100-2 1 1 0 000 2z"></path>
</svg>
  </summary>


  <details-menu class="SelectMenu" role="menu">
    <div class="SelectMenu-modal rounded-3 mt-1" style="max-height:340px;">

        <div class="SelectMenu-filter">
          <input
            class="SelectMenu-input form-control js-filterable-field"
            id="toc-filter-field"
            type="text"
            autocomplete="off"
            spellcheck="false"
            autofocus
            placeholder="Filter headings"
            aria-label="Filter headings">
        </div>

      <div class="SelectMenu-list SelectMenu-list--borderless p-2" style="overscroll-behavior: contain;" data-filterable-for="toc-filter-field" data-filterable-type="substring">
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#master-2-économétrie-et-statistiques-appliquées">MASTER 2 ÉCONOMÉTRIE ET STATISTIQUES APPLIQUÉES</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#svm-et-réseaux-de-neurones">SVM ET RÉSEAUX DE NEURONES</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#classification-dimages-de-sports">CLASSIFICATION D'IMAGES DE SPORTS</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#par">PAR</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#alexandre-gloannec">ALEXANDRE GLOANNEC</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#esteban-pascal">ESTEBAN PASCAL</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#sous-la-direction-de-m-benjamin-roul">SOUS LA DIRECTION DE M. BENJAMIN ROUL</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#février-2023">FÉVRIER 2023</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#problématique-de-létude-de-cas">Problématique de l'étude de cas</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#classification-dimages-de-balles-de-sports">Classification d'images de balles de sports</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#i-importation-du-jeu-de-données">I. Importation du jeu de données</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 24px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#1ère-méthode--importer-les-images-afin-de-les-visualiser">1ère méthode : Importer les images afin de les visualiser</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 24px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#2ème-méthode--importer-les-images-afin-de-les-modéliser">2ème méthode : Importer les images afin de les modéliser</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#ii-data-preparation">II. Data Preparation</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 24px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#anayse-du-jeu-de-données">Anayse du jeu de données</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 24px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#nettoyage-du-jeu-de-données">Nettoyage du jeu de données</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 24px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#standardisation-du-jeu-de-données">Standardisation du jeu de données</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#iii-séparation-de-notre-jeu-de-données-train">III. Séparation de notre jeu de données train</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#iv-modélisation">IV. Modélisation</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 24px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#méthodes-employées-">Méthodes employées :</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--partie-ovr-">- Partie OVR :</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--partie-ovo-">- Partie OVO :</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--mlp-avec-keras">- MLP avec keras</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--arbre-de-décision">- Arbre de décision</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--gradientboostingclassifier">- GradientBoostingClassifier</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--random-forest">- Random Forest</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--ridge-classifier">- Ridge Classifier</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--régression-logistique-multiclass">- Régression Logistique Multiclass</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--partie-ovr">- Partie OVR</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--partie-ovo--1">- Partie OVO :</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--mlp-avec-keras-1">- MLP avec keras</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--arbre-de-décision-1">- Arbre de décision</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--gradientboostingclassifier-1">- GradientBoostingClassifier</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--random-forest-1">- Random Forest</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--ridge-classifier-1">- Ridge Classifier</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 " style="-webkit-box-orient: vertical; padding-left: 36px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#--régression-logistique-multiclass-1">- Régression Logistique Multiclass</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#v-rééchantillonage-des-données">V. Rééchantillonage des données</a>
          <a role="menuitem" class="filter-item SelectMenu-item ws-normal wb-break-word line-clamp-2 py-1 text-emphasized" style="-webkit-box-orient: vertical; padding-left: 12px;" data-action="click:readme-toc#blur" data-targets="readme-toc.entries" data-hydro-click="{&quot;event_type&quot;:&quot;repository_toc_menu.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;entry&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="104e48fbb77695ac931dd7f9efa724ddeced3744ed8197985bd8e9d1d61b5d72" href="#vi-interprétation-du-meilleur-modèle">VI. Interprétation du meilleur modèle</a>
      </div>
    </div>
  </details-menu>
</details>


  <div class="text-mono f6 flex-auto pr-3 flex-order-2 flex-md-order-1">

      352 lines (237 sloc)
      <span class="file-info-divider"></span>
    28.3 KB
  </div>

  <div class="d-flex py-1 py-md-0 flex-auto flex-order-1 flex-md-order-2 flex-sm-grow-0 flex-justify-between hide-sm hide-md">
        <div class="BtnGroup">
      <a href="/estebanpscl/Projet_SVM/blob/main/README.md?plain=1" data-permalink-href="/estebanpscl/Projet_SVM/blob/550d1a20fd36ecc539338565408de5c95fb68d16/README.md?plain=1" aria-label="Display the source blob" data-view-component="true" class="source tooltipped tooltipped tooltipped-n  js-permalink-replaceable-link btn-sm btn BtnGroup-item">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-code">
    <path fill-rule="evenodd" d="M4.72 3.22a.75.75 0 011.06 1.06L2.06 8l3.72 3.72a.75.75 0 11-1.06 1.06L.47 8.53a.75.75 0 010-1.06l4.25-4.25zm6.56 0a.75.75 0 10-1.06 1.06L13.94 8l-3.72 3.72a.75.75 0 101.06 1.06l4.25-4.25a.75.75 0 000-1.06l-4.25-4.25z"></path>
</svg>
</a>      <a href="/estebanpscl/Projet_SVM/blob/main/README.md" data-permalink-href="/estebanpscl/Projet_SVM/blob/550d1a20fd36ecc539338565408de5c95fb68d16/README.md" aria-label="Display the rendered blob" data-view-component="true" class="rendered tooltipped tooltipped tooltipped-n selected js-permalink-replaceable-link btn-sm btn BtnGroup-item">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-file">
    <path fill-rule="evenodd" d="M3.75 1.5a.25.25 0 00-.25.25v12.5c0 .138.112.25.25.25h9.5a.25.25 0 00.25-.25V6h-2.75A1.75 1.75 0 019 4.25V1.5H3.75zm6.75.062V4.25c0 .138.112.25.25.25h2.688a.252.252 0 00-.011-.013l-2.914-2.914a.272.272 0 00-.013-.011zM2 1.75C2 .784 2.784 0 3.75 0h6.586c.464 0 .909.184 1.237.513l2.914 2.914c.329.328.513.773.513 1.237v9.586A1.75 1.75 0 0113.25 16h-9.5A1.75 1.75 0 012 14.25V1.75z"></path>
</svg>
</a>  </div>


    <div class="BtnGroup">
        <a data-permalink-href="/estebanpscl/Projet_SVM/raw/550d1a20fd36ecc539338565408de5c95fb68d16/README.md" href="/estebanpscl/Projet_SVM/raw/main/README.md" id="raw-url" data-view-component="true" class="js-permalink-replaceable-link btn-sm btn BtnGroup-item">    Raw
</a>          <a data-permalink-href="/estebanpscl/Projet_SVM/blame/550d1a20fd36ecc539338565408de5c95fb68d16/README.md" href="/estebanpscl/Projet_SVM/blame/main/README.md" data-hotkey="b" data-view-component="true" class="js-update-url-with-hash js-permalink-replaceable-link btn-sm btn BtnGroup-item">    Blame
</a>    </div>

    <div class="d-flex">
        
<div class="ml-1" >
  <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="BtnGroup-parent js-update-url-with-hash " data-turbo="false" action="/estebanpscl/Projet_SVM/edit/main/README.md" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="4xPCM_8HFHOVzhrDhi46d1OE5DIUTD27M0d3VdfVy7Gyu69HEaHLhDabyKFHN7r-bL3xOxGjGY8tmruGgMLA0w" autocomplete="off" />
      <button title="Edit this file" data-hotkey="e" data-disable-with="" type="submit" data-view-component="true" class="btn-sm BtnGroup-item btn">    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-pencil">
    <path fill-rule="evenodd" d="M11.013 1.427a1.75 1.75 0 012.474 0l1.086 1.086a1.75 1.75 0 010 2.474l-8.61 8.61c-.21.21-.47.364-.756.445l-3.251.93a.75.75 0 01-.927-.928l.929-3.25a1.75 1.75 0 01.445-.758l8.61-8.61zm1.414 1.06a.25.25 0 00-.354 0L10.811 3.75l1.439 1.44 1.263-1.263a.25.25 0 000-.354l-1.086-1.086zM11.189 6.25L9.75 4.81l-6.286 6.287a.25.25 0 00-.064.108l-.558 1.953 1.953-.558a.249.249 0 00.108-.064l6.286-6.286z"></path>
</svg>
</button></form>
  <details class="details-reset details-overlay select-menu BtnGroup-parent d-inline-block position-relative">
      <summary data-disable-invalid="" data-disable-with="" data-dropdown-tracking="{&quot;type&quot;:&quot;blob_edit_dropdown.more_options_click&quot;,&quot;context&quot;:{&quot;repository_id&quot;:599798490,&quot;actor_id&quot;:118008489,&quot;github_dev_enabled&quot;:true,&quot;edit_enabled&quot;:true,&quot;small_screen&quot;:false}}" aria-label="Select additional options" data-view-component="true" class="js-blob-dropdown-click select-menu-button btn-sm btn BtnGroup-item float-none px-2">
</summary>    <div class="SelectMenu right-0">
      <div class="SelectMenu-modal width-full">
        <div class="SelectMenu-list SelectMenu-list--borderless py-2">
          <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="SelectMenu-item js-update-url-with-hash " data-turbo="false" action="/estebanpscl/Projet_SVM/edit/main/README.md" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="IiW-mRldYf1BaOO02Umbiqa4ZQiIK-qhcnN3RGmvphBzjdPt9_u-CuI9MdYYUBsDmYFwAY3EzpVsrruXPritcg" autocomplete="off" />
              <button title="Edit this file" type="submit" data-view-component="true" class="btn-invisible btn width-full d-flex flex-justify-between color-fg-default text-normal p-0">    <div class="mr-5">Edit this file</div>
              <div class="color-fg-muted">E</div>
</button></form>
            <a aria-label="Open this file in github.dev" data-dropdown-tracking="{&quot;type&quot;:&quot;blob_edit_dropdown.dev_link_click&quot;,&quot;context&quot;:{&quot;repository_id&quot;:599798490,&quot;actor_id&quot;:118008489,&quot;edit_enabled&quot;:true,&quot;small_screen&quot;:false}}" href="https://github.dev/" data-view-component="true" class="SelectMenu-item js-github-dev-shortcut js-blob-dropdown-click width-full d-flex flex-justify-between color-fg-default f5 text-normal">
              <div class="mr-5 no-wrap">Open in github.dev</div>
              <div class="color-fg-muted">.</div>
</a>
            <a data-platforms="windows,mac" aria-label="Open this file in GitHub Desktop" href="x-github-client://openRepo/https://github.com/estebanpscl/Projet_SVM?branch=main&amp;filepath=README.md" data-view-component="true" class="SelectMenu-item no-wrap js-remove-unless-platform width-full text-normal color-fg-default f5">
              Open in GitHub Desktop
</a>        </div>
      </div>
    </div>
  </details>
</div>


        
<div >
  <remote-clipboard-copy class="d-inline-block btn-octicon" style="height: 26px" data-src="/estebanpscl/Projet_SVM/raw/550d1a20fd36ecc539338565408de5c95fb68d16/README.md" data-action="click:remote-clipboard-copy#remoteCopy">
  

  <span data-target="remote-clipboard-copy.idle">      <span class="tooltipped tooltipped-nw cursor-pointer" data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;COPY_RAW_CONTENTS_BUTTON&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="6b2f8526d7e62e0e58df3aab1807607cd3dbf531cbe95a02f3b2a82a29c923c1" aria-label="Copy raw contents">
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy">
    <path fill-rule="evenodd" d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 010 1.5h-1.5a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-1.5a.75.75 0 011.5 0v1.5A1.75 1.75 0 019.25 16h-7.5A1.75 1.75 0 010 14.25v-7.5z"></path><path fill-rule="evenodd" d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0114.25 11h-7.5A1.75 1.75 0 015 9.25v-7.5zm1.75-.25a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-7.5a.25.25 0 00-.25-.25h-7.5z"></path>
</svg>
</span></span>
  <span data-target="remote-clipboard-copy.fetching" hidden="hidden">      <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="16" height="16" viewBox="0 0 16 16" fill="none" data-view-component="true" class="anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
</span>
  <span data-target="remote-clipboard-copy.success" hidden="hidden">      <span class="tooltipped tooltipped-nw" aria-label="Copied!">
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check color-fg-success">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
      </span>
</span>
  <span data-target="remote-clipboard-copy.error" hidden="hidden">      <span class="tooltipped tooltipped-nw" aria-label="Something went wrong. Try again.">
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert color-fg-attention">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>
      </span>
</span>
</remote-clipboard-copy></div>


          <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="inline-form" data-turbo="false" action="/estebanpscl/Projet_SVM/delete/main/README.md" accept-charset="UTF-8" method="post"><input type="hidden" name="authenticity_token" value="u38Euw7ttIhcjCfG_ENjkZBuO25bEX24jc2t1lvAOQiotnYOunNAwm8d_Zv7w8YDfVBiSVMNZxt0ZeTGGd4lZQ" />
            <button class="btn-octicon btn-octicon-danger tooltipped tooltipped-nw" type="submit"
              aria-label="Delete this file" data-disable-with>
              <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-trash">
    <path fill-rule="evenodd" d="M6.5 1.75a.25.25 0 01.25-.25h2.5a.25.25 0 01.25.25V3h-3V1.75zm4.5 0V3h2.25a.75.75 0 010 1.5H2.75a.75.75 0 010-1.5H5V1.75C5 .784 5.784 0 6.75 0h2.5C10.216 0 11 .784 11 1.75zM4.496 6.675a.75.75 0 10-1.492.15l.66 6.6A1.75 1.75 0 005.405 15h5.19c.9 0 1.652-.681 1.741-1.576l.66-6.6a.75.75 0 00-1.492-.149l-.66 6.6a.25.25 0 01-.249.225h-5.19a.25.25 0 01-.249-.225l-.66-6.6z"></path>
</svg>
            </button>
</form>    </div>
  </div>

    <div class="d-flex hide-lg hide-xl flex-order-2 flex-grow-0">
      <details class="dropdown details-reset details-overlay d-inline-block">
        <summary
          class="js-blob-dropdown-click btn-octicon p-2"
          aria-haspopup="true"
          aria-label="possible actions"
          
          data-dropdown-tracking="{&quot;type&quot;:&quot;blob_edit_dropdown.more_options_click&quot;,&quot;context&quot;:{&quot;repository_id&quot;:599798490,&quot;actor_id&quot;:118008489,&quot;github_dev_enabled&quot;:true,&quot;edit_enabled&quot;:true,&quot;small_screen&quot;:true}}"
        >
          <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-kebab-horizontal">
    <path d="M8 9a1.5 1.5 0 100-3 1.5 1.5 0 000 3zM1.5 9a1.5 1.5 0 100-3 1.5 1.5 0 000 3zm13 0a1.5 1.5 0 100-3 1.5 1.5 0 000 3z"></path>
</svg>
        </summary>

        <ul class="dropdown-menu dropdown-menu-sw" style="width: 175px">
            <li>
                <a class="dropdown-item tooltipped tooltipped-nw js-remove-unless-platform"
                   data-platforms="windows,mac"
                   href="x-github-client://openRepo/https://github.com/estebanpscl/Projet_SVM?branch=main&amp;filepath=README.md">
                  Open with Desktop
                </a>
            </li>
          <li>
            <a class="dropdown-item" href="/estebanpscl/Projet_SVM/raw/main/README.md">
              View raw
            </a>
          </li>
            <li>
              <remote-clipboard-copy class="dropdown-item" data-src="/estebanpscl/Projet_SVM/raw/main/README.md" data-action="click:remote-clipboard-copy#remoteCopy">
  

  <span data-target="remote-clipboard-copy.idle">                  <span class="cursor-pointer" data-hydro-click="{&quot;event_type&quot;:&quot;repository.click&quot;,&quot;payload&quot;:{&quot;target&quot;:&quot;COPY_RAW_CONTENTS_BUTTON&quot;,&quot;repository_id&quot;:599798490,&quot;originating_url&quot;:&quot;https://github.com/estebanpscl/Projet_SVM/blob/main/README.md&quot;,&quot;user_id&quot;:118008489}}" data-hydro-click-hmac="6b2f8526d7e62e0e58df3aab1807607cd3dbf531cbe95a02f3b2a82a29c923c1">
                    Copy raw contents
</span></span>
  <span data-target="remote-clipboard-copy.fetching" hidden="hidden">                  Copy raw contents
                  <span class="d-inline-block position-relative" style="top: 3px">
                    <svg aria-label="fetching contents…" style="box-sizing: content-box; color: var(--color-icon-primary);" width="16" height="16" viewBox="0 0 16 16" fill="none" data-view-component="true" class="anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
                  </span>
</span>
  <span data-target="remote-clipboard-copy.success" hidden="hidden">                  Copy raw contents
                  <svg aria-label="Copied!" role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check color-fg-success">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
</span>
  <span data-target="remote-clipboard-copy.error" hidden="hidden">                  Copy raw contents
                  <svg aria-label="Something went wrong. Try again." role="img" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert color-fg-attention">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>
</span>
</remote-clipboard-copy>            </li>
            <li>
              <a class="dropdown-item" href="/estebanpscl/Projet_SVM/blame/main/README.md">
                View blame
              </a>
            </li>

              <li class="dropdown-divider" role="none"></li>
              <li>
                <a class="dropdown-item" href="/estebanpscl/Projet_SVM/edit/main/README.md">Edit file</a>
              </li>
                <li>
                  <a data-dropdown-tracking="{&quot;type&quot;:&quot;blob_edit_dropdown.dev_link_click&quot;,&quot;context&quot;:{&quot;repository_id&quot;:599798490,&quot;actor_id&quot;:118008489,&quot;edit_enabled&quot;:true,&quot;small_screen&quot;:true}}" href="https://github.dev/" data-view-component="true" class="dropdown-item js-github-dev-shortcut js-blob-dropdown-click">Open with github.dev</a>
                </li>
              <li>
                <a class="dropdown-item menu-item-danger" href="/estebanpscl/Projet_SVM/delete/main/README.md">Delete file</a>
              </li>
        </ul>
      </details>
    </div>
</div>


        <div id="readme" class="Box-body readme blob js-code-block-container p-5 p-xl-6 gist-border-0">
    <article class="markdown-body entry-content container-lg" itemprop="text"><h1 align="center" dir="auto"><a id="user-content-master-2-économétrie-et-statistiques-appliquées" class="anchor" aria-hidden="true" href="#master-2-économétrie-et-statistiques-appliquées"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>MASTER 2 ÉCONOMÉTRIE ET STATISTIQUES APPLIQUÉES</h1>
<h1 align="center" dir="auto"><a id="user-content-svm-et-réseaux-de-neurones" class="anchor" aria-hidden="true" href="#svm-et-réseaux-de-neurones"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>SVM ET RÉSEAUX DE NEURONES</h1>
<h1 align="center" dir="auto"><a id="user-content-classification-dimages-de-sports" class="anchor" aria-hidden="true" href="#classification-dimages-de-sports"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>CLASSIFICATION D'IMAGES DE SPORTS</h1>
<p align="center" dir="auto">
    <a target="_blank" rel="noopener noreferrer nofollow" href="https://camo.githubusercontent.com/67117f022806d9fde8cb05c1400d2637ee8799cf6ac371ee86c47be7d4e262e9/68747470733a2f2f656e637279707465642d74626e302e677374617469632e636f6d2f696d616765733f713d74626e3a414e6439476354435562583664703530454c4545794f614b6476466b707563496e534d62596f614c324126757371703d434155"><img width="400" src="https://camo.githubusercontent.com/67117f022806d9fde8cb05c1400d2637ee8799cf6ac371ee86c47be7d4e262e9/68747470733a2f2f656e637279707465642d74626e302e677374617469632e636f6d2f696d616765733f713d74626e3a414e6439476354435562583664703530454c4545794f614b6476466b707563496e534d62596f614c324126757371703d434155" alt="reseaux" data-canonical-src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTCUbX6dp50ELEEyOaKdvFkpucInSMbYoaL2A&amp;usqp=CAU" style="max-width: 100%;"></a>
</p>
<h1 align="center" dir="auto"><a id="user-content-par" class="anchor" aria-hidden="true" href="#par"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>PAR</h1>
<h1 align="center" dir="auto"><a id="user-content-alexandre-gloannec" class="anchor" aria-hidden="true" href="#alexandre-gloannec"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>ALEXANDRE GLOANNEC</h1>
<h1 align="center" dir="auto"><a id="user-content-esteban-pascal" class="anchor" aria-hidden="true" href="#esteban-pascal"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>ESTEBAN PASCAL</h1>
<h1 align="center" dir="auto"><a id="user-content-sous-la-direction-de-m-benjamin-roul" class="anchor" aria-hidden="true" href="#sous-la-direction-de-m-benjamin-roul"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>SOUS LA DIRECTION DE M. BENJAMIN ROUL</h1>
<h1 align="center" dir="auto"><a id="user-content-février-2023" class="anchor" aria-hidden="true" href="#février-2023"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>FÉVRIER 2023</h1>
<h1 dir="auto"><a id="user-content-problématique-de-létude-de-cas" class="anchor" aria-hidden="true" href="#problématique-de-létude-de-cas"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a><em><strong>Problématique de l'étude de cas</strong></em></h1>
<h1 dir="auto"><a id="user-content-classification-dimages-de-balles-de-sports" class="anchor" aria-hidden="true" href="#classification-dimages-de-balles-de-sports"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Classification d'images de balles de sports</h1>
<p align="justify" dir="auto">  Le machine learning est la science du développement d'algorithmes et de modèles statistiques que les systèmes informatiques utilisent pour effectuer des tâches sans instructions explicites, en s'appuyant sur des modèles et des déductions. Les systèmes informatiques utilisent des algorithmes de machine learning pour traiter de grandes quantités de données historiques et identifier des modèles de données. Cela leur permet de prédire les résultats avec davantage de précision à partir d'un jeu de données d'entrée donné. Par exemple, les scientifiques des données pourraient entraîner une application médicale en vue de diagnostiquer le cancer à partir d'images radiographiques en stockant des millions d'images numérisées et les diagnostics correspondants. </p>  
<p align="justify" dir="auto"> L'objectif de ce projet a donc été d'appliquer la méthodologie d'un projet de Machine Learning sur un jeu de données concernant la classification d'images de balles de sports. Plus de 6 000 images de ballons de sport de 15 sports différents compose ce jeu de données. Ce sont : le football américain, le baseball, le basketball, la boule de billard, le bowling, la balle de cricket, le football, la balle de golf, la balle de hockey sur gazon, la rondelle de hockey, le ballon de rugby, le volant, la balle de tennis de table, la balle de tennis et le volley-ball. Le projet en question correspond à un projet issu du site Kaggle. Nous avons utilisé la base Kaggle "Sports balls - multiclass image classification". N'ayant pas encore eu l'occasion de travailler avec une classification d'images, nous avons dès lors eu la volonté de nous challenger afin de réaliser un projet différent de ce dont nous avions l'habitude. Néanmoins, excepté durant le cours d'SVM et réseaux de neurones de cette année, nous n'avions jamais travaillé auparavant sur une base de données composée d'images à classifier. Ce qui nous a alors posé quelques problèmes pour l'importation des données puisque lors de ce cours nous avions pu observer l'exemple concernant la base de données "MNIST", cependant l'importation de cette dernière est bien différente de la nôtre. En effet, trouver une solution exploitable pour importer les images nous a pris un certain temps.  Nous avons donc procédé de deux manières : dans un premier temps, une méthode qui a pu nous permettre de visualiser les images de la base de données, mais avec laquelle nous n'avons pas réussi à modéliser. Dans un second temps, une méthode qui nous a cette fois-ci permis de modéliser, mais avec laquelle nous n'avons pas réussi à visualiser les images. Durant ce projet, nous utiliserons donc une combinaison de ces deux méthodes afin de réaliser un modèle de classification multiclass. </p>    
<p dir="auto">Source des données : <a href="https://www.kaggle.com/datasets/samuelcortinhas/sports-balls-multiclass-image-classification" rel="nofollow">https://www.kaggle.com/datasets/samuelcortinhas/sports-balls-multiclass-image-classification</a></p>
<h1 dir="auto"><a id="user-content-i-importation-du-jeu-de-données" class="anchor" aria-hidden="true" href="#i-importation-du-jeu-de-données"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>I. Importation du jeu de données</h1>
<h2 dir="auto"><a id="user-content-1ère-méthode--importer-les-images-afin-de-les-visualiser" class="anchor" aria-hidden="true" href="#1ère-méthode--importer-les-images-afin-de-les-visualiser"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>1ère méthode : Importer les images afin de les visualiser</h2>
<p align="justify" dir="auto"> Dans un premier temps, nous avons mis en place une méthode d'importation des données afin de visualiser les images présentes au sein du jeu de données. Néanmoins, cette méthode ne nous a pas permis de modéliser quoi que ce soit mais nous a aider plus-tard au cours de l'analyse a observer quelles images nos modèles avaient du mal à prédire. </p>  
<p align="justify" dir="auto"> Nous observons ci-dessous à titre d'exemple quelques images ayant pu être visualisées pour 3 catégories de sports différents de manière aléatoire : </p>
<p align="center" dir="auto"> Figure 1 - Image issue de la catégorie baseball </p>
<p align="center" dir="auto">
    <a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/118008489/218047372-31b382ea-d828-4000-a840-8f6fadec111d.png"><img width="400" src="https://user-images.githubusercontent.com/118008489/218047372-31b382ea-d828-4000-a840-8f6fadec111d.png" alt="baseball" style="max-width: 100%;"></a>
</p>
<p align="center" dir="auto"> Source : Gloannec A. &amp; Pascal E. (2023). Classification d'images de balles de sports. Extrait du logiciel Python </p>  
<p align="center" dir="auto"> Figure 2 - Image issue de la catégorie football </p>
<p align="center" dir="auto">
    <a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/118008489/218063229-4beb54fa-7dd0-4562-87f5-c8b354362234.png"><img width="400" src="https://user-images.githubusercontent.com/118008489/218063229-4beb54fa-7dd0-4562-87f5-c8b354362234.png" alt="football" style="max-width: 100%;"></a>
</p>
<p align="center" dir="auto"> Source : Gloannec A. &amp; Pascal E. (2023). Classification d'images de balles de sports. Extrait du logiciel Python </p>
<p align="center" dir="auto"> Figure 3 - Image issue de la catégorie rugby </p>
<p align="center" dir="auto">
    <a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/118008489/218063576-44bb812e-be12-427d-9c46-0c95c37cf5b0.png"><img width="400" src="https://user-images.githubusercontent.com/118008489/218063576-44bb812e-be12-427d-9c46-0c95c37cf5b0.png" alt="rugby" style="max-width: 100%;"></a>
</p>
<p align="center" dir="auto"> Source : Gloannec A. &amp; Pascal E. (2023). Classification d'images de balles de sports. Extrait du logiciel Python </p>
<p align="justify" dir="auto"> Bien que cette méthode soit utile afin d'importer des images, elle n'est pas exploitable pour réaliser une classification. En effet, le premier problème de cette méthode est que les images sont importées sous forme d'une array à 4 dimensions, ce qui rend difficile la modélisation. Le deuxième problème est que nous n'avons pas réussi à exploiter de variables explicatives, ce qui nous aurait ainsi permis de réaliser une classification.
Afin de régler ces problémes, nous avons donc procédé d'une autre manière pour importer nos images. Ce qui nous a donc aider à obtenir des variables explicatives et donc de réaliser notre classification. </p>  
<h2 dir="auto"><a id="user-content-2ème-méthode--importer-les-images-afin-de-les-modéliser" class="anchor" aria-hidden="true" href="#2ème-méthode--importer-les-images-afin-de-les-modéliser"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>2ème méthode : Importer les images afin de les modéliser</h2>
<p align="justify" dir="auto"> Dans un souci de clarté et de temps de calcul pour la performance de notre code, nous avons été obligé de supprimer deux catégories, à savoir "tennis" et "bowling". Après concertation, ces deux catégories à écarter ont été décidés par nous-même.
À noter que plus-tard au cours de l'analyse, nous procéderons à différentes méthodes de rééchantillonage avec nos catégories conservées. </p>  
<p align="justify" dir="auto"> Nous avons essayé de visualiser les images à l'aide du code issue de la démo SVM présente au sein du chapitre 1 concernant les SVM sous python. Nous avons aussi essayé d'autres méthodes mais en vain. </p>
<p align="justify" dir="auto"> Ci-dessous, au sein du tableau 1, nous pouvons tout de même observer la répartition du nombre d'images au sein de chacune des catégories : </p>
<p align="center" dir="auto"> Tableau 1 - Répartition du nombre d'images au sein de chacune des catégories </p>
<div align="center" dir="auto">
<table>
<thead>
<tr>
<th>Catgéories</th>
<th>Images</th>
</tr>
</thead>
<tbody>
<tr>
<td>basketball</td>
<td>340</td>
</tr>
<tr>
<td>billiard_ball</td>
<td>646</td>
</tr>
<tr>
<td>cricket_ball</td>
<td>581</td>
</tr>
<tr>
<td>football</td>
<td>604</td>
</tr>
<tr>
<td>golf_ball</td>
<td>549</td>
</tr>
<tr>
<td>hockey_puck</td>
<td>690</td>
</tr>
<tr>
<td>rugby_ball</td>
<td>493</td>
</tr>
<tr>
<td>shuttlecock</td>
<td>429</td>
</tr>
<tr>
<td>table_tennis_ball</td>
<td>620</td>
</tr>
<tr>
<td>volleyball</td>
<td>432</td>
</tr>
</tbody>
</table>
</div>  
<p align="center" dir="auto"> Source : Gloannec A. &amp; Pascal E. (2023). Classification d'images de balles de sports. </p>
<p align="justify" dir="auto">  La répartition des images présentes au sein de chaque catégorie est sensiblement égale entre chaque catégorie. Ainsi, un rééchantillonage de notre jeu de données n'est a priori pas nécessaire, mais par souci d'analyse approfondie, nos modélisations, qui seront présentées dans la partie suivante, seront à la fois réalisées avec et sans rééchantillonage de notre jeu de données.  </p>  
<h1 dir="auto"><a id="user-content-ii-data-preparation" class="anchor" aria-hidden="true" href="#ii-data-preparation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>II. Data Preparation</h1>
<h2 dir="auto"><a id="user-content-anayse-du-jeu-de-données" class="anchor" aria-hidden="true" href="#anayse-du-jeu-de-données"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Anayse du jeu de données</h2>
<ul dir="auto">
<li>Analyse des variables (Variable d'intérêt / Variables explicatives)</li>
<li>Identification des valeurs manquantes</li>
<li>Identification et correction des outliers</li>
</ul>
<h2 dir="auto"><a id="user-content-nettoyage-du-jeu-de-données" class="anchor" aria-hidden="true" href="#nettoyage-du-jeu-de-données"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Nettoyage du jeu de données</h2>
<ul dir="auto">
<li>Imputation de valeurs manquantes</li>
</ul>
<h2 dir="auto"><a id="user-content-standardisation-du-jeu-de-données" class="anchor" aria-hidden="true" href="#standardisation-du-jeu-de-données"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Standardisation du jeu de données</h2>
<p align="justify" dir="auto"> Étant donné notre jeu de données composé d'images à classifier, l'ensemble des étapes énoncées ci-dessous au sein de la partie consacrée à la préparation des données n'ont pas été / pu être réalisées. Le cas échéant, celles-ci auraient du être développées de manière rigoureuse.
C'est pour cette raison que nous sommes directement passé à notre étape de modélisation. </p>  
<h1 dir="auto"><a id="user-content-iii-séparation-de-notre-jeu-de-données-train" class="anchor" aria-hidden="true" href="#iii-séparation-de-notre-jeu-de-données-train"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>III. Séparation de notre jeu de données train</h1>
<p align="justify" dir="auto"> La validation croisée est une technique d’apprentissage supervisé pour vérifier la fiabilité d’un modèle. </p>  
<p align="justify" dir="auto"> Ici nous utlisons la validation croisée Hold Out pour séparer notre jeu train en deux nouvelles bases : </p>  
<p align="justify" dir="auto"> - Un échantillon d’apprentissage pour entraîner les paramètres du modèle. </p> 
<p align="justify" dir="auto"> - Un échantillon de validation pour vérifier la déviance du modèle. </p> 
<p align="justify" dir="auto"> Le split du jeu de données s'est effectué de la manière suivante : 80% du jeu de données en jeu train et 20% du jeu de données en jeu test. </p>  
<h1 dir="auto"><a id="user-content-iv-modélisation" class="anchor" aria-hidden="true" href="#iv-modélisation"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>IV. Modélisation</h1>
<p align="justify" dir="auto"> Nous allons maintenant présenter la modélisation et les résultats obtenus en termes de performance pour chacun de nos modèles choisis dans cette étude avec nos catégories retenues. À noter que nous présenterons pour chacun de nos modèles à la fois les résultats de nos modélisations obtenus sans rééchantillonage et avec rééchantillonage du jeu de données. </p>  
<p align="justify" dir="auto"> Concernant les méthodes que nous avons employé durant cette étude de cas, voici l'ordre dans lequel celles-ci ont été mises en place : </p>  
<h2 dir="auto"><a id="user-content-méthodes-employées-" class="anchor" aria-hidden="true" href="#méthodes-employées-"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>Méthodes employées :</h2>
<h3 dir="auto"><a id="user-content---partie-ovr-" class="anchor" aria-hidden="true" href="#--partie-ovr-"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- Partie OVR :</h3>
<ul dir="auto">
<li>OneVSRestClassifier (SVC)</li>
<li>OneVsRestClassifier (LinearSVC)</li>
<li>OneVsRestClassifier (SGDClassifier)</li>
</ul>
<h3 dir="auto"><a id="user-content---partie-ovo-" class="anchor" aria-hidden="true" href="#--partie-ovo-"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- Partie OVO :</h3>
<ul dir="auto">
<li>OneVsOneClassifier (SVC)</li>
<li>OneVsOneClassifier (LinearSVC)</li>
<li>OneVsOneClassifier (SGDClassifier)</li>
</ul>
<h3 dir="auto"><a id="user-content---mlp-avec-keras" class="anchor" aria-hidden="true" href="#--mlp-avec-keras"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- MLP avec keras</h3>
<h3 dir="auto"><a id="user-content---arbre-de-décision" class="anchor" aria-hidden="true" href="#--arbre-de-décision"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- Arbre de décision</h3>
<h3 dir="auto"><a id="user-content---gradientboostingclassifier" class="anchor" aria-hidden="true" href="#--gradientboostingclassifier"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- GradientBoostingClassifier</h3>
<h3 dir="auto"><a id="user-content---random-forest" class="anchor" aria-hidden="true" href="#--random-forest"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- Random Forest</h3>
<h3 dir="auto"><a id="user-content---ridge-classifier" class="anchor" aria-hidden="true" href="#--ridge-classifier"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- Ridge Classifier</h3>
<h3 dir="auto"><a id="user-content---régression-logistique-multiclass" class="anchor" aria-hidden="true" href="#--régression-logistique-multiclass"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- Régression Logistique Multiclass</h3>
<p align="justify" dir="auto"> Et voici la démarche suivie pour cette partie concernant la modélisation : </p>  
<ul dir="auto">
<li>Application des modèles à l’échantillon test.</li>
<li>Comparaison de la performance des modèles (Matrice de confusion, Accuracy).</li>
</ul>
<p align="justify" dir="auto"> Nous introduirons tout d'abord chaque méthode avant de présenter à la fin de cette partie un tableau récapitulatif résumant pour chacune d'entre elles à la fois, la qualité de prévision du modèle, ainsi que le nombre de fois ou le modèle prédit d'une mauvaise manière les images pour chaque catégorie </p>    
<h3 dir="auto"><a id="user-content---partie-ovr" class="anchor" aria-hidden="true" href="#--partie-ovr"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- Partie OVR</h3>
<ul dir="auto">
<li>OneVsRestClassifier (SVC)</li>
<li>OneVsRestClassifier (LinearSVC)</li>
<li>OneVsRestClassifier (SGDClassifier)</li>
</ul>
<p align="justify" dir="auto"> Stratégie multiclass/multilabel OneVSRestClassifier (OVR), également connue sous le nom de OneVSAll. Cette approche consiste à ajuster un classifieur par classe. Pour chaque classificateur, la classe est ajustée par rapport à toutes les autres classes. En plus de son efficacité de calcul (seuls les classificateurs n_classes sont nécessaires), l'un des avantages de cette approche est son interprétabilité. Étant donné que chaque classe est représentée par un et un seul classificateur, il est possible d'acquérir des connaissances sur la classe en inspectant son classificateur correspondant. Il s'agit de la stratégie la plus couramment utilisée pour la classification multiclasse et c'est un choix par défaut équitable. </p>  
<h3 dir="auto"><a id="user-content---partie-ovo--1" class="anchor" aria-hidden="true" href="#--partie-ovo--1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- Partie OVO :</h3>
<ul dir="auto">
<li>OneVsOneClassifier (SVC)</li>
<li>OneVsOneClassifier (LinearSVC)</li>
<li>OneVsOneClassifier (SGDClassifier)</li>
</ul>
<p align="justify" dir="auto"> OneVsOneClassifier construit un classificateur par paire de classes. Au moment de la prédiction, la classe qui a reçu le plus de votes est sélectionnée. En cas d'égalité (entre deux classes avec un nombre égal de votes), il sélectionne la classe avec la confiance de classification agrégée la plus élevée en additionnant les niveaux de confiance de classification par paire calculés par les classificateurs binaires sous-jacents. Puisqu'elle nécessite d'adapter n_classes * (n_classes - 1) / 2 classificateurs, cette méthode est généralement plus lente que OneVSRestClassifier, en raison de sa complexité O (n_classes^2). La fonction de décision est le résultat d'une transformation monotone de la classification un contre un. </p>  
<h3 dir="auto"><a id="user-content---mlp-avec-keras-1" class="anchor" aria-hidden="true" href="#--mlp-avec-keras-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- MLP avec keras</h3>
<p align="justify" dir="auto"> En intelligence artificielle, plus précisément en apprentissage automatique, le perceptron multicouche (multilayer perceptron, MLP) est un type de réseau neuronal artificiel organisé en plusieurs couches. L'information circule de la couche d'entrée vers la couche de sortie uniquement : il s'agit donc d'un réseau à propagation directe (feedforward). Chaque couche est constituée d'un nombre variable de neurones, les neurones de la dernière couche (dite « de sortie ») étant les sorties du système global. </p>  
<p align="justify" dir="auto"> Malheureusement nous n'avons pas réussi à obtenir quelconque résultat interprétable à l'aide de la méthode MLP avec Keras.  
Cependant, nous avons souhaité tester d'autres modèles que ceux vus en cous. Par conséquent, nous avons décidé du choix de ces modèles à l'aide de la documentation suivante : <a href="https://scikit-learn.org/stable/modules/multiclass.html" rel="nofollow">https://scikit-learn.org/stable/modules/multiclass.html</a> </p> 
<h3 dir="auto"><a id="user-content---arbre-de-décision-1" class="anchor" aria-hidden="true" href="#--arbre-de-décision-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- Arbre de décision</h3>
 <p align="justify" dir="auto"> Un arbre de décision est un outil d'aide à la décision représentant un ensemble de choix sous la forme graphique d'un arbre. Les différentes décisions possibles sont situées aux extrémités des branches (les « feuilles » de l'arbre), et sont atteintes en fonction de décisions prises à chaque étape. L'arbre de décision est un outil utilisé dans des domaines variés tels que la sécurité, la fouille de données, la médecine, etc. Il a l'avantage d'être lisible et rapide à exécuter. Il s'agit de plus d'une représentation calculable automatiquement par des algorithmes d'apprentissage supervisé. </p>  
<h3 dir="auto"><a id="user-content---gradientboostingclassifier-1" class="anchor" aria-hidden="true" href="#--gradientboostingclassifier-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- GradientBoostingClassifier</h3>
<p align="justify" dir="auto"> Le gradient boosting est un modèle ensembliste de boosting utilisant la descente de gradient pour optimiser une fonction de perte. Cette descente est utilisée pour le calcul des résidus des individus, lors de la construction du modèle suivant.  
Cette méthode est implémentée dans la librairie scikit-learn : GradientBoostingRegressor et GradientBoostingClassifier. </p>  
<p align="justify" dir="auto"> Au sujet du modèle GradientBoostingClassifier, celui-ci a nécessité un nombre conséquent de temps de calcul rien qu'avec 3 catégories afin de tester le modèle. C'est pourquoi nous n'avons pu malheureusement l'appliquer à l'ensemble de nos catégories et l'avons alors mis de côté. </p>  
<h3 dir="auto"><a id="user-content---random-forest-1" class="anchor" aria-hidden="true" href="#--random-forest-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- Random Forest</h3>
<p align="justify" dir="auto"> Le Random Forest est un modèle ensembliste basé sur la construction de multiples arbres de décision (CART).
Chaque arbre est construit à partir d’un échantillon aléatoire avec remise des individus et des variables. Lors d’une classification, la prédiction finale est la modalité majoritairement prédite. </p>  
<p align="justify" dir="auto"> Les avantages sont les suivants : 
</p><ul dir="auto">
<li>Accepte les variables qualitatives et quantitatives</li>
<li>Pas besoin de vérifier des hypothèses de normalité et de variance</li>
<li>Il répond aux problèmes de classification et régression</li>
<li>Modèle relativement puissant sur des problèmes de modélisation complexe <p dir="auto"></p></li>
</ul>
<p align="justify" dir="auto"> Tandis que les inconvénients sont :  
</p><ul dir="auto">
<li>Difficilement interprétable</li>
<li>Attention au sur-apprentissage <p dir="auto"></p></li>
</ul>
<h3 dir="auto"><a id="user-content---ridge-classifier-1" class="anchor" aria-hidden="true" href="#--ridge-classifier-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- Ridge Classifier</h3>
<p align="justify" dir="auto"> En apprentissage automatique, la classification ridge est une technique utilisée pour analyser les modèles discriminants linéaires. C'est une forme de régularisation qui pénalise les coefficients du modèle pour éviter le surajustement. Le surajustement est un problème courant dans l'apprentissage automatique qui se produit lorsqu'un modèle est trop complexe et capture le bruit dans les données au lieu du signal sous-jacent. Cela peut conduire à de mauvaises performances de généralisation sur de nouvelles données. La classification Ridge résout ce problème en ajoutant un terme de pénalité à la fonction de coût qui décourage la complexité. Il en résulte un modèle plus apte à généraliser à de nouvelles données.  </p>  
<h3 dir="auto"><a id="user-content---régression-logistique-multiclass-1" class="anchor" aria-hidden="true" href="#--régression-logistique-multiclass-1"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>- Régression Logistique Multiclass</h3>
<p align="justify" dir="auto"> La régression logistique est une technique d'analyse de données qui utilise les mathématiques pour trouver les relations entre deux facteurs de données. Elle utilise ensuite cette relation pour prédire la valeur de l'un de ces facteurs en fonction de l'autre. La régression logistique est une technique importante dans le domaine de l'intelligence artificielle et du machine learning. Les modèles de régression logistique peuvent traiter de grands volumes de données à grande vitesse, car ils nécessitent moins de capacité de calcul, comme la mémoire et la puissance de traitement. </p>   
<p align="justify" dir="auto"> Il est important de savoir qu'afin de réaliser une classification multiclass avec une régression logistique, nous avons précisé au sein des paramètres l'argument multi_class = "multinomial". </p>
<p align="justify" dir="auto"> Pour l'ensemble des méthodes, hormis la régression logistique, les paramètres par défaut des modèles ont été utilisés. D'autre part, nous n'avons pas pu mettre en place les méthodes de GridSearch et RandomozidesGridSearch pour notre modélisation. À nouveau, la problématique du temps de calcul de ces méthodes pour nos données est rentrée en compte. </p>
<h1 dir="auto"><a id="user-content-v-rééchantillonage-des-données" class="anchor" aria-hidden="true" href="#v-rééchantillonage-des-données"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>V. Rééchantillonage des données</h1>
<p align="justify" dir="auto"> Précédemment, nous avons vu que certaines catégories étaient malgré tout sous-représentées vis-à-vis de certaines.  Nous allons donc procéder à de l'undersumpling afin d'améliorer potentiellement la qualité de nos modèles. Le sous-échantillonnage implique d'introduire un biais pour sélectionner plus d'échantillons d'une classe que d'une autre, afin de compenser un déséquilibre déjà présent dans les données ou susceptible de se développer si un échantillon purement aléatoire était prélevé. </p>  
<p align="justify" dir="auto"> À noter que nous n'avons pas procédé également à de l'oversampling car cette méthode prenait beaucoup trop de temps de calcul dans le cas de notre analyse. C'est la raison pour laquelle nous avons concentré nos efforts sur l'undersampling. </p>  
<p align="justify" dir="auto">  Voici donc au sein de la figure 4 la nouvelle répartition après Undersampling de nos données : </p>    
<p align="center" dir="auto"> Figure 4 - Nouvelle répartition après Undersampling de nos données </p>
<p align="center" dir="auto">
    <a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/118008489/218097925-50b38942-c9c1-494f-883a-e25031580641.png"><img width="400" src="https://user-images.githubusercontent.com/118008489/218097925-50b38942-c9c1-494f-883a-e25031580641.png" alt="undersampling" style="max-width: 100%;"></a>
</p>
<p align="center" dir="auto"> Source : Gloannec A. &amp; Pascal E. (2023). Classification d'images de balles de sports. Extrait du logiciel Python </p>
<p align="justify" dir="auto"> Ci-dessous, au sein du tableau 2, nous observons la nouvelle répartition du nombre d'images au sein de chacune des catégories après undersampling: </p>
<p align="center" dir="auto"> Tableau 2 - Répartition du nombre d'images au sein de chacune des catégories après undersampling </p>
<div align="center" dir="auto">
<table>
<thead>
<tr>
<th>Catgéories</th>
<th>Images</th>
</tr>
</thead>
<tbody>
<tr>
<td>american_football</td>
<td>340</td>
</tr>
<tr>
<td>baseball</td>
<td>340</td>
</tr>
<tr>
<td>basketball</td>
<td>340</td>
</tr>
<tr>
<td>billiard_ball</td>
<td>340</td>
</tr>
<tr>
<td>bowling_ball</td>
<td>340</td>
</tr>
<tr>
<td>cricket_ball</td>
<td>340</td>
</tr>
<tr>
<td>football</td>
<td>340</td>
</tr>
<tr>
<td>golf_ball</td>
<td>340</td>
</tr>
<tr>
<td>hockey_ball</td>
<td>340</td>
</tr>
<tr>
<td>hockey_puck</td>
<td>340</td>
</tr>
<tr>
<td>rugby_ball</td>
<td>340</td>
</tr>
<tr>
<td>shuttlecock</td>
<td>340</td>
</tr>
<tr>
<td>table_tennis_ball</td>
<td>340</td>
</tr>
<tr>
<td>volleyball</td>
<td>340</td>
</tr>
</tbody>
</table>
</div>  
<p align="center" dir="auto"> Source : Gloannec A. &amp; Pascal E. (2023). Classification d'images de balles de sports. </p>
<p align="center" dir="auto">  Cette fois-ci le nombre de catégories est supérieure étant donné qu'avec la procédure d'Undersampling nous ne rencontrons plus de problème quant à la richesse de notre base de données. </p>
<p align="justify" dir="auto"> Sans oublier que nous séparons dans ce cas ci-présent aussi notre jeu train en deux nouveaux jeux de données pour la modélisation : 80% du jeu de données en jeu train et 20% du jeu de données en jeu test. </p>  
<h1 dir="auto"><a id="user-content-vi-interprétation-du-meilleur-modèle" class="anchor" aria-hidden="true" href="#vi-interprétation-du-meilleur-modèle"><svg class="octicon octicon-link" viewBox="0 0 16 16" version="1.1" width="16" height="16" aria-hidden="true"><path fill-rule="evenodd" d="M7.775 3.275a.75.75 0 001.06 1.06l1.25-1.25a2 2 0 112.83 2.83l-2.5 2.5a2 2 0 01-2.83 0 .75.75 0 00-1.06 1.06 3.5 3.5 0 004.95 0l2.5-2.5a3.5 3.5 0 00-4.95-4.95l-1.25 1.25zm-4.69 9.64a2 2 0 010-2.83l2.5-2.5a2 2 0 012.83 0 .75.75 0 001.06-1.06 3.5 3.5 0 00-4.95 0l-2.5 2.5a3.5 3.5 0 004.95 4.95l1.25-1.25a.75.75 0 00-1.06-1.06l-1.25 1.25a2 2 0 01-2.83 0z"></path></svg></a>VI. Interprétation du meilleur modèle</h1>
<p align="justify" dir="auto"> Enfin, passons au récapitulatif des résultats en termes de performances de l'ensemble des modèles. Nous représentons au sein du tableau 3 la qualité de prévision de l'ensemble des modèles. Notons que nous ne pouvons comparer les qualités de prévision entre les deux méthodes. Tandis qu'au sein des tableaux 4 et 5, c'est le nombre d'erreur réalisé pour le meilleur modèle, avant et après rééchantillonage, comme image mal prédite pour chaque catégorie que nous observons. Enfin, les tableaux 6 et 7 montrent les matrices de confusion obtenues pour la méthode Random Forest avant et après rééchantillonage. </p>
<p align="center" dir="auto"> Tableau 3 - Qualité de prévision de l'ensemble des modèles </p>
<div align="center" dir="auto">
<table>
<thead>
<tr>
<th>Modèles</th>
<th>Avant rééchantillonage</th>
<th>Après rééchantillonage</th>
</tr>
</thead>
<tbody>
<tr>
<td>OneVSRestClassifier (SVC)</td>
<td>49,16%</td>
<td>44,66%</td>
</tr>
<tr>
<td>OneVsRestClassifier (LinearSVC)</td>
<td>39,23%</td>
<td>34,14%</td>
</tr>
<tr>
<td>OneVsRestClassifier (SGDClassifier)</td>
<td>29,79%</td>
<td>20,25%</td>
</tr>
<tr>
<td>OneVSOneClassifier (SVC)</td>
<td>41,79%</td>
<td>34,72%</td>
</tr>
<tr>
<td>OneVsOneClassifier (LinearSVC)</td>
<td>41,79%</td>
<td>37,28%</td>
</tr>
<tr>
<td>OneVsOneClassifier (SGDClassifier)</td>
<td>31,66%</td>
<td>26,83%</td>
</tr>
<tr>
<td>Arbre de décision</td>
<td>32,35%</td>
<td>29,16%</td>
</tr>
<tr>
<td>Random Forest</td>
<td>51,23%</td>
<td>47,66%</td>
</tr>
<tr>
<td>Ridge Classifier</td>
<td>36,97%</td>
<td>31,94%</td>
</tr>
<tr>
<td>Régression Logistique Multiclass</td>
<td>26,70%</td>
<td>25,95%</td>
</tr>
</tbody>
</table>
</div>  
<p align="center" dir="auto"> Source : Gloannec A. &amp; Pascal E. (2023). Classification d'images de balles de sports. </p>
<p align="center" dir="auto"> Tableau 4 - Nombre d'erreur réalisé pour le modèle Random Forest avant rééchantillonage comme image mal prédite pour chaque catégorie </p>
<div align="center" dir="auto">
<table>
<thead>
<tr>
<th></th>
<th>Random Forest</th>
</tr>
</thead>
<tbody>
<tr>
<td>basketball</td>
<td>46</td>
</tr>
<tr>
<td>billiard_ball</td>
<td>39</td>
</tr>
<tr>
<td>cricket_ball</td>
<td>36</td>
</tr>
<tr>
<td>football</td>
<td>69</td>
</tr>
<tr>
<td>golf_ball</td>
<td>60</td>
</tr>
<tr>
<td>hockey_puck</td>
<td>43</td>
</tr>
<tr>
<td>rugby_ball</td>
<td>50</td>
</tr>
<tr>
<td>shuttlecock</td>
<td>38</td>
</tr>
<tr>
<td>table_tennis_ball</td>
<td>51</td>
</tr>
<tr>
<td>volleyball</td>
<td>64</td>
</tr>
</tbody>
</table>
</div>  
<p align="center" dir="auto"> Source : Gloannec A. &amp; Pascal E. (2023). Classification d'images de balles de sports. </p>
<p align="center" dir="auto"> Tableau 5 - Nombre d'erreur réalisé pour le modèle Random Forest après rééchantillonage comme image mal prédite pour chaque catégorie </p>
<div align="center" dir="auto">
<table>
<thead>
<tr>
<th></th>
<th>Random Forest</th>
</tr>
</thead>
<tbody>
<tr>
<td>american_football</td>
<td>53</td>
</tr>
<tr>
<td>baseball</td>
<td>61</td>
</tr>
<tr>
<td>basketball</td>
<td>32</td>
</tr>
<tr>
<td>billiard_ball</td>
<td>56</td>
</tr>
<tr>
<td>bowling_ball</td>
<td>48</td>
</tr>
<tr>
<td>cricket_ball</td>
<td>40</td>
</tr>
<tr>
<td>football</td>
<td>61</td>
</tr>
<tr>
<td>golf_ball</td>
<td>61</td>
</tr>
<tr>
<td>hockey_ball</td>
<td>52</td>
</tr>
<tr>
<td>hockey_puck</td>
<td>49</td>
</tr>
<tr>
<td>rugby_ball</td>
<td>57</td>
</tr>
<tr>
<td>shuttlecock</td>
<td>33</td>
</tr>
<tr>
<td>table_tennis_ball</td>
<td>54</td>
</tr>
<tr>
<td>volleyball</td>
<td>65</td>
</tr>
</tbody>
</table>
</div>  
<p align="center" dir="auto"> Source : Gloannec A. &amp; Pascal E. (2023). Classification d'images de balles de sports. </p>
<p align="center" dir="auto"> Tableau 6 - Matrice de confusion du modèle Random Forest avant rééchantillonage </p>
<p align="center" dir="auto">
    <a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/118008489/218124162-c0676566-4454-43d2-b6db-e3d4765ad1d9.png"><img width="800" src="https://user-images.githubusercontent.com/118008489/218124162-c0676566-4454-43d2-b6db-e3d4765ad1d9.png" alt="matrice" style="max-width: 100%;"></a>
</p>
<p align="center" dir="auto"> Source : Gloannec A. &amp; Pascal E. (2023). Classification d'images de balles de sports. Extrait du logiciel Python </p>
<p align="center" dir="auto"> Tableau 7 - Matrice de confusion du modèle Random Forest après rééchantillonage </p>
<p align="center" dir="auto">
    <a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/118008489/218125518-3d0ad316-23d3-4ff2-92f4-60af366d8146.png"><img width="800" src="https://user-images.githubusercontent.com/118008489/218125518-3d0ad316-23d3-4ff2-92f4-60af366d8146.png" alt="matrice1" style="max-width: 100%;"></a>
    <a target="_blank" rel="noopener noreferrer nofollow" href="https://user-images.githubusercontent.com/118008489/218125644-c677a28e-ccea-4b08-b619-c13ab8709e8d.png"><img width="400" src="https://user-images.githubusercontent.com/118008489/218125644-c677a28e-ccea-4b08-b619-c13ab8709e8d.png" alt="matrice2" style="max-width: 100%;"></a>
</p>
<p align="center" dir="auto"> Source : Gloannec A. &amp; Pascal E. (2023). Classification d'images de balles de sports. Extrait du logiciel Python </p>
<p align="justify" dir="auto"> Pour conclure cette analyse concernant la classification d'images de balles de sports, il s'avère que le meilleur modèle obtenu pour classifier ces dernières de manière optimale s'avère être le modèle Random Forest, avant et après rééchantillonage, avec une qualité de prévision, respectivement, de 51,23% et 47,66%. Ce modèle prédit donc correctement les images de balles de sports pour chacune des catégories dans environ 50% des cas. </p>  
<p align="justify" dir="auto"> Au sujet du nombre d'erreur réalisé pour le modèle Random Forest avant rééchantillonage comme image mal prédite pour chaque catégorie, le modèle réalise le minimum d'erreur pour les catégories billiard_ball, cricket_ball et shuttlecock avec, respectivement, 39 erreurs, 36 erreurs et 38 erreurs. À l'inverse, le modèle réalise le maximum d'erreur pour les catégories football et volleyball, avec 69 erreurs pour l'une contre 64 erreurs pour l'autre.</p>  
<p align="justify" dir="auto"> Par ailleurs, pour le nombre d'erreur réalisé pour le modèle Random Forest après rééchantillonage comme image mal prédite pour chaque catégorie, le modèle réalise le minimum d'erreur pour les catégories basketball et shuttlecock, avec 32 erreurs pour l'une contre 33 erreurs pour l'autre. À l'inverse, le modèle réalise le maximum d'erreur pour les catégories baseball, football, golf_ball et volleyball avec 61 erreurs pour les 3 premières contre 65 erreurs pour la dernière.</p>  
<p align="justify" dir="auto"> Pour approfondir les précédentes observations, nous décidons alors d'observer les matrices de confusion du modèle Random Forest avant et après rééchantillonage. </p>   
<p align="justify" dir="auto"> Pour la première matrice de confusion, avant rééchantillonage, certes le modèle prédit la catégorie billiard_ball comme étant l'une d'entre elles avec le plus petit nombre d'erreur d'image mal prédite. Seulement, a contrario des catégories cricket_ball et shuttlecock, elles aussi très performantes, le modèle a tendance à prédire beaucoup d'autres balles de sport comme étant des boules de billard. Cela peut notamment s'expliquer du fait que la boule de billard soit ronde et que notre base de données en contient beaucoup de cette forme, au contraire de forme de balles telles que les balles de cricket et de volant de badminton. En effet, les catégories les moins bien prédites sont le football et le volleyball, ce qui coincide. </p>   
<p align="justify" dir="auto"> Pour la seconde matrice de confusion, après rééchantillonage, le constat semble être le même. Des balles de sport rondes apparaissent comme étant les moins bien prédites, hormis pour les balles de basketball étant très bien prédites. De plus, le modèle se trompe souvent en associant des balles de sport rondes à des boules de billard. </p>   
</article>
  </div>

    </div>

  </readme-toc>

  

  <details class="details-reset details-overlay details-overlay-dark" id="jumpto-line-details-dialog">
    <summary data-hotkey="l" aria-label="Jump to line"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast linejump overflow-hidden" aria-label="Jump to line">
      <!-- '"` --><!-- </textarea></xmp> --></option></form><form class="js-jump-to-line-form Box-body d-flex" data-turbo="false" action="" accept-charset="UTF-8" method="get">
        <input class="form-control flex-auto mr-3 linejump-input js-jump-to-line-field" type="text" placeholder="Jump to line&hellip;" aria-label="Jump to line" autofocus>
          <button data-close-dialog="" type="submit" data-view-component="true" class="btn">    Go
</button>
</form>    </details-dialog>
  </details>



    <div class="pt-3" >
      <details class="details-reset details-overlay details-overlay-dark " >
                <summary data-view-component="true" class="btn-link">    Give feedback
</summary>

  <details-dialog
    class="Box d-flex flex-column anim-fade-in fast Box--overlay overflow-visible"
      aria-label="Provide feedback"
      src="/estebanpscl/Projet_SVM/repos/code_nav_survey"
      
    >
    <div class="Box-header">
      <button class="Box-btn-octicon btn-octicon float-right" type="button" aria-label="Close dialog" data-close-dialog>
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg>
      </button>
        <h1 class="Box-title" >Provide feedback</h1>
    </div>
      <div class="Box-body overflow-auto">
                  <include-fragment>
            <svg style="box-sizing: content-box; color: var(--color-icon-primary);" width="32" height="32" viewBox="0 0 16 16" fill="none" data-view-component="true" class="my-3 mx-auto d-block anim-rotate">
  <circle cx="8" cy="8" r="7" stroke="currentColor" stroke-opacity="0.25" stroke-width="2" vector-effect="non-scaling-stroke" />
  <path d="M15 8a7.002 7.002 0 00-7-7" stroke="currentColor" stroke-width="2" stroke-linecap="round" vector-effect="non-scaling-stroke" />
</svg>
          </include-fragment>

      </div>
  </details-dialog>
</details>
    </div>
</div>

  </div>


  </div>

  </turbo-frame>


    </main>
  </div>

  </div>

          <footer class="footer width-full container-xl p-responsive">
  <h2 class='sr-only'>Footer</h2>

  <div class="position-relative d-flex flex-items-center pb-2 f6 color-fg-muted border-top color-border-muted flex-column-reverse flex-lg-row flex-wrap flex-lg-nowrap mt-6 pt-6">
    <div class="list-style-none d-flex flex-wrap col-0 col-lg-2 flex-justify-start flex-lg-justify-between mb-2 mb-lg-0">
      <div class="mt-2 mt-lg-0 d-flex flex-items-center">
        <a aria-label="Homepage" title="GitHub" class="footer-octicon mr-2" href="https://github.com">
          <svg aria-hidden="true" height="24" viewBox="0 0 16 16" version="1.1" width="24" data-view-component="true" class="octicon octicon-mark-github">
    <path fill-rule="evenodd" d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.013 8.013 0 0016 8c0-4.42-3.58-8-8-8z"></path>
</svg>
</a>        <span>
        &copy; 2023 GitHub, Inc.
        </span>
      </div>
    </div>

    <nav aria-label='footer' class="col-12 col-lg-8">
      <h3 class='sr-only' id='sr-footer-heading'>Footer navigation</h3>
      <ul class="list-style-none d-flex flex-wrap col-12 flex-justify-center flex-lg-justify-between mb-2 mb-lg-0" aria-labelledby='sr-footer-heading'>
          <li class="mr-3 mr-lg-0"><a href="https://docs.github.com/site-policy/github-terms/github-terms-of-service" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to terms&quot;,&quot;label&quot;:&quot;text:terms&quot;}">Terms</a></li>
          <li class="mr-3 mr-lg-0"><a href="https://docs.github.com/site-policy/privacy-policies/github-privacy-statement" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to privacy&quot;,&quot;label&quot;:&quot;text:privacy&quot;}">Privacy</a></li>
          <li class="mr-3 mr-lg-0"><a data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to security&quot;,&quot;label&quot;:&quot;text:security&quot;}" href="https://github.com/security">Security</a></li>
          <li class="mr-3 mr-lg-0"><a href="https://www.githubstatus.com/" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to status&quot;,&quot;label&quot;:&quot;text:status&quot;}">Status</a></li>
          <li class="mr-3 mr-lg-0"><a data-ga-click="Footer, go to help, text:Docs" href="https://docs.github.com">Docs</a></li>
          <li class="mr-3 mr-lg-0"><a href="https://support.github.com?tags=dotcom-footer" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to contact&quot;,&quot;label&quot;:&quot;text:contact&quot;}">Contact GitHub</a></li>
          <li class="mr-3 mr-lg-0"><a href="https://github.com/pricing" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to Pricing&quot;,&quot;label&quot;:&quot;text:Pricing&quot;}">Pricing</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://docs.github.com" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to api&quot;,&quot;label&quot;:&quot;text:api&quot;}">API</a></li>
        <li class="mr-3 mr-lg-0"><a href="https://services.github.com" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to training&quot;,&quot;label&quot;:&quot;text:training&quot;}">Training</a></li>
          <li class="mr-3 mr-lg-0"><a href="https://github.blog" data-analytics-event="{&quot;category&quot;:&quot;Footer&quot;,&quot;action&quot;:&quot;go to blog&quot;,&quot;label&quot;:&quot;text:blog&quot;}">Blog</a></li>
          <li><a data-ga-click="Footer, go to about, text:about" href="https://github.com/about">About</a></li>
      </ul>
    </nav>
  </div>

  <div class="d-flex flex-justify-center pb-6">
    <span class="f6 color-fg-muted"></span>
  </div>
</footer>




  <div id="ajax-error-message" class="ajax-error-message flash flash-error" hidden>
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>
    <button type="button" class="flash-close js-ajax-error-dismiss" aria-label="Dismiss error">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg>
    </button>
    You can’t perform that action at this time.
  </div>

  <div class="js-stale-session-flash flash flash-warn flash-banner" hidden
    >
    <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-alert">
    <path fill-rule="evenodd" d="M8.22 1.754a.25.25 0 00-.44 0L1.698 13.132a.25.25 0 00.22.368h12.164a.25.25 0 00.22-.368L8.22 1.754zm-1.763-.707c.659-1.234 2.427-1.234 3.086 0l6.082 11.378A1.75 1.75 0 0114.082 15H1.918a1.75 1.75 0 01-1.543-2.575L6.457 1.047zM9 11a1 1 0 11-2 0 1 1 0 012 0zm-.25-5.25a.75.75 0 00-1.5 0v2.5a.75.75 0 001.5 0v-2.5z"></path>
</svg>
    <span class="js-stale-session-flash-signed-in" hidden>You signed in with another tab or window. <a href="">Reload</a> to refresh your session.</span>
    <span class="js-stale-session-flash-signed-out" hidden>You signed out in another tab or window. <a href="">Reload</a> to refresh your session.</span>
  </div>
    <template id="site-details-dialog">
  <details class="details-reset details-overlay details-overlay-dark lh-default color-fg-default hx_rsm" open>
    <summary role="button" aria-label="Close dialog"></summary>
    <details-dialog class="Box Box--overlay d-flex flex-column anim-fade-in fast hx_rsm-dialog hx_rsm-modal">
      <button class="Box-btn-octicon m-0 btn-octicon position-absolute right-0 top-0" type="button" aria-label="Close dialog" data-close-dialog>
        <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-x">
    <path fill-rule="evenodd" d="M3.72 3.72a.75.75 0 011.06 0L8 6.94l3.22-3.22a.75.75 0 111.06 1.06L9.06 8l3.22 3.22a.75.75 0 11-1.06 1.06L8 9.06l-3.22 3.22a.75.75 0 01-1.06-1.06L6.94 8 3.72 4.78a.75.75 0 010-1.06z"></path>
</svg>
      </button>
      <div class="octocat-spinner my-6 js-details-dialog-spinner"></div>
    </details-dialog>
  </details>
</template>

    <div class="Popover js-hovercard-content position-absolute" style="display: none; outline: none;" tabindex="0">
  <div class="Popover-message Popover-message--bottom-left Popover-message--large Box color-shadow-large" style="width:360px;">
  </div>
</div>

    <template id="snippet-clipboard-copy-button">
  <div class="zeroclipboard-container position-absolute right-0 top-0">
    <clipboard-copy aria-label="Copy" class="ClipboardButton btn js-clipboard-copy m-2 p-0 tooltipped-no-delay" data-copy-feedback="Copied!" data-tooltip-direction="w">
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-copy js-clipboard-copy-icon m-2">
    <path fill-rule="evenodd" d="M0 6.75C0 5.784.784 5 1.75 5h1.5a.75.75 0 010 1.5h-1.5a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-1.5a.75.75 0 011.5 0v1.5A1.75 1.75 0 019.25 16h-7.5A1.75 1.75 0 010 14.25v-7.5z"></path><path fill-rule="evenodd" d="M5 1.75C5 .784 5.784 0 6.75 0h7.5C15.216 0 16 .784 16 1.75v7.5A1.75 1.75 0 0114.25 11h-7.5A1.75 1.75 0 015 9.25v-7.5zm1.75-.25a.25.25 0 00-.25.25v7.5c0 .138.112.25.25.25h7.5a.25.25 0 00.25-.25v-7.5a.25.25 0 00-.25-.25h-7.5z"></path>
</svg>
      <svg aria-hidden="true" height="16" viewBox="0 0 16 16" version="1.1" width="16" data-view-component="true" class="octicon octicon-check js-clipboard-check-icon color-fg-success d-none m-2">
    <path fill-rule="evenodd" d="M13.78 4.22a.75.75 0 010 1.06l-7.25 7.25a.75.75 0 01-1.06 0L2.22 9.28a.75.75 0 011.06-1.06L6 10.94l6.72-6.72a.75.75 0 011.06 0z"></path>
</svg>
    </clipboard-copy>
  </div>
</template>


    <style>
      .user-mention[href$="/estebanpscl"] {
        color: var(--color-user-mention-fg);
        background-color: var(--color-user-mention-bg);
        border-radius: 2px;
        margin-left: -2px;
        margin-right: -2px;
        padding: 0 2px;
      }
    </style>


    </div>

    <div id="js-global-screen-reader-notice" class="sr-only" aria-live="polite" ></div>
  </body>
</html>

