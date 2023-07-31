# Comparing `tmp/open_rarity-0.7.2.tar.gz` & `tmp/open-rarity-1.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_rarity-0.7.2.tar", max compression
+gzip compressed data, was "open-rarity-1.0.0a1.tar", max compression
```

## Comparing `open_rarity-0.7.2.tar` & `open-rarity-1.0.0a1.tar`

### file list

```diff
@@ -1,43 +1,40 @@
--rw-r--r--   0        0        0    11325 2023-07-17 07:45:34.380673 open_rarity-0.7.2/LICENSE
--rw-r--r--   0        0        0     3964 2023-07-17 07:45:34.380673 open_rarity-0.7.2/README.md
--rw-r--r--   0        0        0      247 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/data/__init__.py
--rw-r--r--   0        0        0     3729 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/data/test_collections.json
--rw-r--r--   0        0        0      256 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/models/__init__.py
--rw-r--r--   0        0        0      143 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/models/chain.py
--rw-r--r--   0        0        0    11362 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/models/collection.py
--rw-r--r--   0        0        0     5172 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/models/token.py
--rw-r--r--   0        0        0     2298 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/models/token_identifier.py
--rw-r--r--   0        0        0     7621 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/models/token_metadata.py
--rw-r--r--   0        0        0      341 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/models/token_ranking_features.py
--rw-r--r--   0        0        0      657 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/models/token_rarity.py
--rw-r--r--   0        0        0      521 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/models/token_standard.py
--rw-r--r--   0        0        0        0 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/models/utils/__init__.py
--rw-r--r--   0        0        0      501 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/models/utils/attribute_utils.py
--rw-r--r--   0        0        0     4173 2023-07-27 08:03:49.911217 open_rarity-0.7.2/open_rarity/rarity_ranker.py
--rw-r--r--   0        0        0        0 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/resolver/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/resolver/models/__init__.py
--rw-r--r--   0        0        0      390 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/resolver/models/collection_with_metadata.py
--rw-r--r--   0        0        0      823 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/resolver/models/token_with_rarity_data.py
--rw-r--r--   0        0        0    15709 2023-07-27 08:03:49.911217 open_rarity-0.7.2/open_rarity/resolver/opensea_api_helpers.py
--rw-r--r--   0        0        0        0 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/resolver/rarity_providers/__init__.py
--rw-r--r--   0        0        0    12983 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/resolver/rarity_providers/external_rarity_provider.py
--rw-r--r--   0        0        0      273 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/resolver/rarity_providers/rank_resolver.py
--rw-r--r--   0        0        0     2553 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/resolver/rarity_providers/rarity_sniffer.py
--rw-r--r--   0        0        0     1855 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/resolver/rarity_providers/rarity_sniper.py
--rw-r--r--   0        0        0     5309 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/resolver/rarity_providers/trait_sniper.py
--rw-r--r--   0        0        0    24992 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/resolver/testset_resolver.py
--rw-r--r--   0        0        0       27 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/scoring/__init__.py
--rw-r--r--   0        0        0        0 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/scoring/handlers/__init__.py
--rw-r--r--   0        0        0     2637 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/scoring/handlers/arithmetic_mean_scoring_handler.py
--rw-r--r--   0        0        0     2785 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/scoring/handlers/geometric_mean_scoring_handler.py
--rw-r--r--   0        0        0     2693 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/scoring/handlers/harmonic_mean_scoring_handler.py
--rw-r--r--   0        0        0     9190 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/scoring/handlers/information_content_scoring_handler.py
--rw-r--r--   0        0        0      186 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/scoring/handlers/scoring_handlers.md
--rw-r--r--   0        0        0     2613 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/scoring/handlers/sum_scoring_handler.py
--rw-r--r--   0        0        0     4054 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/scoring/scorer.py
--rw-r--r--   0        0        0     1676 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/scoring/scoring_handler.py
--rw-r--r--   0        0        0     1242 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/scoring/token_feature_extractor.py
--rw-r--r--   0        0        0     3544 2023-07-17 07:45:34.392672 open_rarity-0.7.2/open_rarity/scoring/utils.py
--rw-r--r--   0        0        0     1490 2023-07-27 08:04:02.535246 open_rarity-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     4961 1970-01-01 00:00:00.000000 open_rarity-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11325 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/LICENSE
+-rw-r--r--   0        0        0     4930 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/README.md
+-rw-r--r--   0        0        0      117 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/cli/__init__.py
+-rw-r--r--   0        0        0     1280 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/cli/main.py
+-rw-r--r--   0        0        0     3554 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/cli/opensea.py
+-rw-r--r--   0        0        0      362 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/cli/utils.py
+-rw-r--r--   0        0        0       77 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/collection/__init__.py
+-rw-r--r--   0        0        0    10884 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/collection/collection.py
+-rw-r--r--   0        0        0      427 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/collection/types.py
+-rw-r--r--   0        0        0     2990 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/collection/utils.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/io/__init__.py
+-rw-r--r--   0        0        0      284 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/io/read.py
+-rw-r--r--   0        0        0      291 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/io/write.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/metrics/__init__.py
+-rw-r--r--   0        0        0     1169 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/metrics/ic.py
+-rw-r--r--   0        0        0     1054 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/metrics/trait_count.py
+-rw-r--r--   0        0        0       53 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/providers/__init__.py
+-rw-r--r--   0        0        0       60 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/providers/opensea/__init__.py
+-rw-r--r--   0        0        0     5951 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/providers/opensea/client.py
+-rw-r--r--   0        0        0      279 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/providers/opensea/types.py
+-rw-r--r--   0        0        0    20524 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/providers/testset_resolver.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/py.typed
+-rw-r--r--   0        0        0      109 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/token/__init__.py
+-rw-r--r--   0        0        0       56 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/token/metadata/__init__.py
+-rw-r--r--   0        0        0       85 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/token/metadata/dtypes/__init__.py
+-rw-r--r--   0        0        0     2640 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/token/metadata/dtypes/number.py
+-rw-r--r--   0        0        0     1055 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/token/metadata/dtypes/string.py
+-rw-r--r--   0        0        0     5333 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/token/metadata/metadata.py
+-rw-r--r--   0        0        0     1764 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/token/token.py
+-rw-r--r--   0        0        0     2043 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/token/types.py
+-rw-r--r--   0        0        0      678 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/types.py
+-rw-r--r--   0        0        0       35 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/utils/__init__.py
+-rw-r--r--   0        0        0      935 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/utils/aio.py
+-rw-r--r--   0        0        0     2816 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/utils/data.py
+-rw-r--r--   0        0        0        0 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/validators/__init__.py
+-rw-r--r--   0        0        0      550 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/openrarity/validators/string.py
+-rw-r--r--   0        0        0     1644 2022-11-17 17:06:51.000000 open-rarity-1.0.0a1/pyproject.toml
+-rw-r--r--   0        0        0     6385 1970-01-01 00:00:00.000000 open-rarity-1.0.0a1/setup.py
+-rw-r--r--   0        0        0     6103 1970-01-01 00:00:00.000000 open-rarity-1.0.0a1/PKG-INFO
```

### Comparing `open_rarity-0.7.2/LICENSE` & `open-rarity-1.0.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `open_rarity-0.7.2/open_rarity/resolver/testset_resolver.py` & `open-rarity-1.0.0a1/openrarity/providers/testset_resolver.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,692 +1,555 @@
-import argparse
-import csv
-import io
-import json
-import logging
-import math
-import os
-import pkgutil
-from dataclasses import dataclass
-from time import strftime, time
-from typing import Iterable
-
-import numpy as np
-
-from open_rarity.models.collection import Collection
-from open_rarity.models.token import Token
-from open_rarity.models.token_identifier import EVMContractTokenIdentifier
-from open_rarity.models.token_rarity import TokenRarity
-from open_rarity.rarity_ranker import RarityRanker
-from open_rarity.resolver.models.collection_with_metadata import CollectionWithMetadata
-from open_rarity.resolver.models.token_with_rarity_data import (
-    RankProvider,
-    RarityData,
-    TokenWithRarityData,
-)
-from open_rarity.resolver.opensea_api_helpers import (
-    get_collection_with_metadata_from_opensea,
-)
-from open_rarity.resolver.rarity_providers.external_rarity_provider import (
-    EXTERNAL_RANK_PROVIDERS,
-    ExternalRarityProvider,
-)
-from open_rarity.scoring.handlers.arithmetic_mean_scoring_handler import (
-    ArithmeticMeanScoringHandler,
-)
-from open_rarity.scoring.handlers.geometric_mean_scoring_handler import (
-    GeometricMeanScoringHandler,
-)
-from open_rarity.scoring.handlers.harmonic_mean_scoring_handler import (
-    HarmonicMeanScoringHandler,
-)
-from open_rarity.scoring.handlers.information_content_scoring_handler import (
-    InformationContentScoringHandler,
-)
-from open_rarity.scoring.handlers.sum_scoring_handler import SumScoringHandler
-from open_rarity.scoring.token_feature_extractor import TokenFeatureExtractor
-
-harmonic_handler = HarmonicMeanScoringHandler()
-arithmetic_handler = ArithmeticMeanScoringHandler()
-geometric_handler = GeometricMeanScoringHandler()
-sum_handler = SumScoringHandler()
-ic_handler = InformationContentScoringHandler()
-
-RankScore = tuple[int, float]
-# Token ID -> Score
-ScoredTokens = dict[int, float]
-# Token ID -> Rank + Score
-RankedTokens = dict[int, RankScore]
-
-logger = logging.getLogger("open_rarity_logger")
-
-
-parser = argparse.ArgumentParser()
-parser.add_argument(
-    "resolve_external_rarity",
-    type=str,
-    default="external",
-    help="Specify 'external' if you want to resolve rarity from external providers",
-)
-parser.add_argument(
-    "--cache",
-    dest="cache_fetched_data",
-    action=argparse.BooleanOptionalAction,
-    default=True,
-    help="Whether we use local data files to cache external trait + rank data",
-)
-parser.add_argument(
-    "--filename",
-    dest="filename",
-    default="test_collections.json",
-    help="File in /data folder containing collections to resolve.",
-)
-
-# The fastest external rarity provider, taking <15 seconds to resolve all rank data.
-parser.add_argument(
-    "--rarity_sniffer",
-    dest="fetch_rarity_sniffer",
-    action=argparse.BooleanOptionalAction,
-    default=True,
-    help="If external is specified, fetches rarity sniffer ranking data",
-)
-
-# Default disabled due to API key requirements. Without caching, this can take
-# ~10 minutes for a 10k collection due to rate limits.
-parser.add_argument(
-    "--trait_sniper",
-    dest="fetch_trait_sniper",
-    action=argparse.BooleanOptionalAction,
-    default=False,
-    help=(
-        "If external is specified, fetches trait sniper ranking data. "
-        "If True, must set TRAIT_SNIPER_API_KEY env var."
-    ),
-)
-
-# Default disabled because no public bulk fetcher function and therefore
-# takes a long to fetch data for (~25 min for 10k collection).
-parser.add_argument(
-    "--rarity_sniper",
-    dest="fetch_rarity_sniper",
-    action=argparse.BooleanOptionalAction,
-    default=False,
-    help="If external is specified, fetches rarity sniper ranking data",
-)
-
-
-@dataclass
-class OpenRarityScores:
-    arithmetic_scores: RankedTokens
-    geometric_scores: RankedTokens
-    harmonic_scores: RankedTokens
-    sum_scores: RankedTokens
-    information_content_scores: RankedTokens
-
-
-def get_tokens_with_rarity(
-    collection_with_metadata: CollectionWithMetadata,
-    external_rank_providers: list[RankProvider] = EXTERNAL_RANK_PROVIDERS,
-    resolve_remote_rarity: bool = True,
-    batch_size: int = 300,
-    max_tokens_to_calculate: int = None,
-    cache_external_ranks: bool = True,
-) -> list[TokenWithRarityData]:
-    """Resolves assets through OpenSea API asset endpoint and turns them
-    into token with rarity data, augmented with rankings from Gem, RaritySniper
-    and TraitSniper.
-
-    Parameters
-    ----------
-    collection : Collection
-        collection
-    resolve_remote_rarity : bool
-        True if we need to resolve rarity ranks from
-        external providers , False if not
-    max_tokens_to_calculate (int, optional): If specified only gets ranking
-        data of first `max_tokens`. Defaults to None.
-    cache_external_ranks : bool
-        If set to true, will cache external ranks into local json file and
-        optionally use cached data if file exists. If cache file already exists,
-        will not refetch or rewrite cache data.
-
-    Returns
-    -------
-    list[TokenWithRarityData]
-        provide list of tokens augmented with assets metadata and ranking provider
-    """
-    slug = collection_with_metadata.opensea_slug
-    external_rarity_provider = ExternalRarityProvider()
-    total_supply = min(
-        max_tokens_to_calculate or collection_with_metadata.token_total_supply,
-        collection_with_metadata.token_total_supply,
-    )
-    num_batches = math.ceil(total_supply / batch_size)
-    tokens = collection_with_metadata.collection.tokens
-    if len(tokens) != collection_with_metadata.token_total_supply:
-        # TODO [open-rarity] - Add support for collections with skipped token ids
-        msg = (
-            f"Warning: Collection {slug} has {len(tokens)} tokens, but total supply "
-            f"is {collection_with_metadata.token_total_supply}. This can happen if "
-            f"the collection skips token IDs. "
-        )
-        logger.warning(msg)
-        print(msg)
-    tokens_with_rarity: list[TokenWithRarityData] = []
-
-    t1_start = time()
-
-    tokens_batch: Iterable[Token]
-    for batch_id, tokens_batch in enumerate(
-        np.array_split(tokens, num_batches)  # type: ignore
-    ):
-        message = (
-            f"\tStarting batch {batch_id} for collection "
-            f"{slug}: Processing {len(tokens_batch)} tokens. "
-            f"Last token: {tokens_batch[-1]}"
-        )
-        logger.debug(message)
-        print(message)
-
-        # We will store all rarities calculated across providers in this list
-        tokens_rarity_batch = [
-            TokenWithRarityData(token=t, rarities=[]) for t in tokens_batch
-        ]
-
-        if resolve_remote_rarity:
-            external_rarity_provider.fetch_and_update_ranks(
-                collection_with_metadata=collection_with_metadata,
-                tokens_with_rarity=tokens_rarity_batch,
-                rank_providers=external_rank_providers,
-                cache_external_ranks=cache_external_ranks,
-            )
-        # Add the batch of augmented tokens with rarity into return value
-        tokens_with_rarity.extend(tokens_rarity_batch)
-
-    t1_stop = time()
-    logger.debug(
-        "Elapsed time during the asset resolution in seconds {seconds}".format(
-            seconds=t1_stop - t1_start
-        )
-    )
-
-    return tokens_with_rarity
-
-
-def resolve_collection_data(
-    resolve_remote_rarity: bool,
-    external_rank_providers: list[RankProvider],
-    package_path: str = "open_rarity.data",
-    filename: str = "test_collections.json",
-    max_tokens_to_calculate: int = None,
-    use_cache: bool = True,
-    output_file_to_disk: bool = True,
-) -> list | None:
-    """Resolves collection information through OpenSea API
-
-    Parameters
-    ----------
-    resolve_remote_rarity : bool
-        Set to true to resolve external rarity ranks for rank comparisons
-    package_path : str, optional
-        The package path for where the collection data to resolve collection data lives,
-        by default "open_rarity.data"
-    filename : str, optional
-        The filename of the file holding the collection slugs to resolve,
-        by default "test_collections.json"
-    max_tokens_to_calculate : int, optional
-        If specified only gets ranking data of first `max_tokens`, by default None.
-        Note: If this is provided, we cannot calculate OpenRarity ranks since
-        it must be calculated after calculating scoring for entire collection.
-    use_cache: bool
-        If set to true, will cache fetched data from external API's in order to ensure
-        re-runs for same collections are faster. Only use if collection and token
-        metadata is static - do not work for unrevealed/changing collections.
-    output_file_to_disk: bool
-        If set to true, will output the resolved collection data to disk.
-        Set to False if you want to use the data in memory only.
-        Needed for testing.
-
-    Returns
-    -------
-    list
-        A list of the rows that would be written to the output file. Only returned if
-        output_file_to_disk is set to False.
-
-    Raises
-    ------
-    ValueError
-        If the file containing collection slugs to resolve does not exist.
-    """
-    golden_collections = pkgutil.get_data(package_path, filename)
-    if not golden_collections:
-        raise ValueError("Can't resolve golden collections data file.")
-
-    data = json.load(io.BytesIO(golden_collections))
-    print("------------------------------")
-    output_rows: list = []
-    for collection_def in data:
-        start_time = time()
-        opensea_slug = collection_def["collection_slug"]
-        print(f"\nBEGIN: Resolving collection {opensea_slug}")
-        print(
-            f"1. Fetching collection & token traits for: {opensea_slug} from opensea."
-        )
-        # Fetch collection metadata and tokens that belong to this collection
-        # from opensea and other external api's.
-        collection_with_metadata = get_collection_with_metadata_from_opensea(
-            opensea_collection_slug=opensea_slug,
-            use_cache=use_cache,
-        )
-        print(f"2. Fetching external rarity ranks for: {opensea_slug}")
-        tokens_with_rarity: list[TokenWithRarityData] = get_tokens_with_rarity(
-            collection_with_metadata=collection_with_metadata,
-            resolve_remote_rarity=resolve_remote_rarity,
-            max_tokens_to_calculate=max_tokens_to_calculate,
-            cache_external_ranks=use_cache,
-            external_rank_providers=external_rank_providers,
-        )
-        print(f"3. Calculating OpenRarity ranks for: {opensea_slug}")
-
-        collection = collection_with_metadata.collection
-
-        if max_tokens_to_calculate is None:
-            assert collection.token_total_supply == len(tokens_with_rarity)
-        else:
-            assert max_tokens_to_calculate == len(tokens_with_rarity)
-
-        # Calculate and append open rarity scores
-        if max_tokens_to_calculate is None:
-            open_rarity_scores = resolve_open_rarity_score(
-                collection, collection.tokens
-            )
-            augment_with_open_rarity_scores(
-                tokens_with_rarity=tokens_with_rarity,
-                scores=open_rarity_scores,
-            )
-
-        if output_file_to_disk:
-            print(f"4. Wrote to CSV: {opensea_slug}")
-
-        rows = serialize_to_csv(
-            collection_with_metadata=collection_with_metadata,
-            tokens_with_rarity=tokens_with_rarity,
-            dry_run=not output_file_to_disk,
-        )
-        if rows is not None:
-            output_rows += rows
-        time_elapsed = round(time() - start_time)
-        print(f"FINISHED: Resolved collection: {opensea_slug} in {time_elapsed} secs")
-
-    return output_rows if not output_file_to_disk else None
-
-
-def augment_with_open_rarity_scores(
-    tokens_with_rarity: list[TokenWithRarityData], scores: OpenRarityScores
-) -> None:
-    """Augments tokens_with_rarity with ranks and scores computed by
-    OpenRarity scorers'"""
-    for token_with_rarity in tokens_with_rarity:
-        token_id = token_with_rarity.token.token_identifier.token_id  # type: ignore
-
-        token_with_rarity.rarities.extend(
-            [
-                RarityData(
-                    provider=RankProvider.OR_ARITHMETIC,
-                    rank=scores.arithmetic_scores[token_id][0],
-                    score=scores.arithmetic_scores[token_id][1],
-                ),
-                RarityData(
-                    provider=RankProvider.OR_GEOMETRIC,
-                    rank=scores.geometric_scores[token_id][0],
-                    score=scores.geometric_scores[token_id][1],
-                ),
-                RarityData(
-                    provider=RankProvider.OR_HARMONIC,
-                    rank=scores.harmonic_scores[token_id][0],
-                    score=scores.harmonic_scores[token_id][1],
-                ),
-                RarityData(
-                    provider=RankProvider.OR_SUM,
-                    rank=scores.sum_scores[token_id][0],
-                    score=scores.sum_scores[token_id][1],
-                ),
-                RarityData(
-                    provider=RankProvider.OR_INFORMATION_CONTENT,
-                    rank=scores.information_content_scores[token_id][0],
-                    score=scores.information_content_scores[token_id][1],
-                ),
-            ]
-        )
-
-
-def extract_rank(tokens_to_score: dict[str, TokenRarity]) -> RankedTokens:
-    """Sorts dictionary by float score and extract rank according to the score
-
-    Parameters
-    ----------
-    token_id_to_scores : dict[str, TokenRarity]
-        dictionary of token_id_to_scores with token_id to score mapping
-
-    Returns
-    -------
-    dict[str, RankScore]
-        dictionary of token to rank, score pair
-    """
-    ranked_tokens: list[TokenRarity] = RarityRanker.set_rarity_ranks(
-        token_rarities=list(tokens_to_score.values())
-    )
-
-    result = {}
-    for token in ranked_tokens:
-        assert token.rank
-        # note: this is a bug, ignoring the mypy error for now
-        # token_identifier can be of type SolanaMintAddressTokenIdentifier
-        # which has no token_id
-        result[int(token.token.token_identifier.token_id)] = (  # type: ignore
-            token.rank,
-            token.score,
-        )
-    return result
-
-
-def resolve_open_rarity_score(
-    collection: Collection, tokens: list[Token]
-) -> OpenRarityScores:
-    """Resolve scores from all scorers with trait_normalization
-
-    Parameters
-    ----------
-    collection : Collection
-        collection is needed since the score is based on the invdividual's traits
-        probability across the entire collection
-    tokens: Subset of tokens belonging to Collection to resolve open rarity scores for
-
-    """
-    t1_start = time()
-
-    # Dictionaries of token IDs to their respective TokenRarity for each strategy
-    arthimetic_dict: dict[str, TokenRarity] = {}
-    geometric_dict: dict[str, TokenRarity] = {}
-    harmonic_dict: dict[str, TokenRarity] = {}
-    sum_dict: dict[str, TokenRarity] = {}
-    ic_dict: dict[str, TokenRarity] = {}
-
-    logger.debug("OpenRarity scoring")
-
-    for token in tokens:
-        token_identifier = token.token_identifier
-        assert isinstance(token_identifier, EVMContractTokenIdentifier)
-        token_id = str(token_identifier.token_id)
-
-        try:
-            token_features = TokenFeatureExtractor.extract_unique_attribute_count(
-                token=token, collection=collection
-            )
-
-            harmonic_dict[token_id] = TokenRarity(
-                token=token,
-                token_features=token_features,
-                score=harmonic_handler.score_token(collection=collection, token=token),
-            )
-            arthimetic_dict[token_id] = TokenRarity(
-                token=token,
-                token_features=token_features,
-                score=arithmetic_handler.score_token(
-                    collection=collection, token=token
-                ),
-            )
-            geometric_dict[token_id] = TokenRarity(
-                token=token,
-                token_features=token_features,
-                score=geometric_handler.score_token(collection=collection, token=token),
-            )
-            sum_dict[token_id] = TokenRarity(
-                token=token,
-                token_features=token_features,
-                score=sum_handler.score_token(collection=collection, token=token),
-            )
-            ic_dict[token_id] = TokenRarity(
-                token=token,
-                token_features=token_features,
-                score=ic_handler.score_token(collection=collection, token=token),
-            )
-
-        except Exception:
-            logger.exception(f"Can't score token {token} with OpenRarity")
-
-    # Calculate ranks of all assets given the scores
-    arthimetic_ranked_tokens = extract_rank(arthimetic_dict)
-    geometric_ranked_tokens = extract_rank(geometric_dict)
-    harmonic_ranked_tokens = extract_rank(harmonic_dict)
-    sum_ranked_tokens = extract_rank(sum_dict)
-    ic_ranked_tokens = extract_rank(ic_dict)
-
-    t1_stop = time()
-    logger.debug(
-        "OpenRarity scores resolution in seconds {seconds}".format(
-            seconds=t1_stop - t1_start
-        )
-    )
-
-    return OpenRarityScores(
-        arithmetic_scores=arthimetic_ranked_tokens,
-        geometric_scores=geometric_ranked_tokens,
-        harmonic_scores=harmonic_ranked_tokens,
-        sum_scores=sum_ranked_tokens,
-        information_content_scores=ic_ranked_tokens,
-    )
-
-
-def _get_provider_rank(
-    provider: RankProvider, token_with_rarity: TokenWithRarityData
-) -> int | None:
-    """Get rank for the particular provider
-
-    Parameters
-    ----------
-    provider : RankProvider
-        rank provider
-    token : Token
-        token
-    """
-    rarities = token_with_rarity.rarities
-    rarity_datas = list(filter(lambda rarity: rarity.provider == provider, rarities))
-    return rarity_datas[0].rank if len(rarity_datas) > 0 else None
-
-
-def _rank_diff(rank1: int | None, rank2: int | None) -> int | None:
-    """Function that computes the rank difference
-
-    Parameters
-    ----------
-    rank1 : int | None
-        rank of the asset
-    rank2 : int | None
-        rank of the asset
-
-    Returns
-    -------
-    int | None
-        absolute difference of ranks for the specific asset
-    """
-    if not rank1 or not rank2:
-        return None
-
-    return abs(rank1 - rank2)
-
-
-def serialize_to_csv(
-    collection_with_metadata: CollectionWithMetadata,
-    tokens_with_rarity: list[TokenWithRarityData],
-    dry_run: bool = False,
-) -> list | None:
-    """Serialize collection and ranking data to CSV
-
-    Parameters
-    ----------
-    collection_with_metadata : Collection
-    dry_run: bool
-        If set to True, the CSV will not be written to disk but returned as an
-        array of rows
-
-    """
-    slug = collection_with_metadata.opensea_slug
-    testset = open(f"testset_{slug}.csv", "w")
-    headers = [
-        "slug",
-        "token_id",
-        "traits_sniper",
-        "rarity_sniffer",
-        "rarity_sniper",
-        "arithmetic",
-        "geometric",
-        "harmonic",
-        "sum",
-        "information_content",
-        "traits_sniper_rarity_sniffer_diff",
-        "traits_sniper_rarity_sniper_diff",
-        "traits_sniper_arithm_diff",
-        "traits_sniper_geom_diff",
-        "traits_sniper_harmo_diff",
-        "traits_sniper_sum_diff",
-        "traits_sniper_ic_diff",
-        "rarity_sniffer_rarity_sniper_diff",
-        "rarity_sniffer_arithm_diff",
-        "rarity_sniffer_geom_diff",
-        "rarity_sniffer_harmo_diff",
-        "rarity_sniffer_sum_diff",
-        "rarity_sniffer_ic_diff",
-        "rarity_sniper_arithm_diff",
-        "rarity_sniper_geom_diff",
-        "rarity_sniper_harmo_diff",
-        "rarity_sniper_sum_diff",
-        "rarity_sniper_ic_diff",
-    ]
-
-    writer = csv.writer(testset)
-    writer.writerow(headers)
-    rows = []
-
-    for token_with_rarity in tokens_with_rarity:
-        traits_sniper_rank = _get_provider_rank(
-            RankProvider.TRAITS_SNIPER, token_with_rarity
-        )
-        rarity_sniffer_rank = _get_provider_rank(
-            RankProvider.RARITY_SNIFFER, token_with_rarity
-        )
-        rarity_sniper_rank = _get_provider_rank(
-            RankProvider.RARITY_SNIPER, token_with_rarity
-        )
-        or_arithmetic_rank = _get_provider_rank(
-            RankProvider.OR_ARITHMETIC, token_with_rarity
-        )
-        or_geometric_rank = _get_provider_rank(
-            RankProvider.OR_GEOMETRIC, token_with_rarity
-        )
-        or_harmonic_rank = _get_provider_rank(
-            RankProvider.OR_HARMONIC, token_with_rarity
-        )
-        or_sum_rank = _get_provider_rank(RankProvider.OR_SUM, token_with_rarity)
-        or_ic_rank = _get_provider_rank(
-            RankProvider.OR_INFORMATION_CONTENT, token_with_rarity
-        )
-        row = [
-            slug,
-            token_with_rarity.token.token_identifier.token_id,  # type: ignore
-            traits_sniper_rank,
-            rarity_sniffer_rank,
-            rarity_sniper_rank,
-            or_arithmetic_rank,
-            or_geometric_rank,
-            or_harmonic_rank,
-            or_sum_rank,
-            or_ic_rank,
-            _rank_diff(traits_sniper_rank, rarity_sniffer_rank),
-            _rank_diff(traits_sniper_rank, rarity_sniper_rank),
-            _rank_diff(traits_sniper_rank, or_arithmetic_rank),
-            _rank_diff(traits_sniper_rank, or_geometric_rank),
-            _rank_diff(traits_sniper_rank, or_harmonic_rank),
-            _rank_diff(traits_sniper_rank, or_sum_rank),
-            _rank_diff(traits_sniper_rank, or_ic_rank),
-            _rank_diff(rarity_sniffer_rank, rarity_sniper_rank),
-            _rank_diff(rarity_sniffer_rank, or_arithmetic_rank),
-            _rank_diff(rarity_sniffer_rank, or_geometric_rank),
-            _rank_diff(rarity_sniffer_rank, or_harmonic_rank),
-            _rank_diff(rarity_sniffer_rank, or_sum_rank),
-            _rank_diff(rarity_sniffer_rank, or_ic_rank),
-            _rank_diff(rarity_sniper_rank, or_arithmetic_rank),
-            _rank_diff(rarity_sniper_rank, or_geometric_rank),
-            _rank_diff(rarity_sniper_rank, or_harmonic_rank),
-            _rank_diff(rarity_sniper_rank, or_sum_rank),
-            _rank_diff(rarity_sniper_rank, or_ic_rank),
-        ]
-        if dry_run:
-            rows.append(row)
-        else:
-            writer.writerow(row)
-
-    return rows if rows else None
-
-
-if __name__ == "__main__":
-    """Script to resolve external datasets and compute rarity scores
-    on test collections. Data resolved from opensea api
-
-    Command to run:
-    `python -m open_rarity.resolver.testset_resolver external`
-
-        This will only produce ranks from OpenRarity and RaritySniffer by default.
-
-    To run for all external providers:
-    `TRAIT_SNIPER_API_KEY=<your key> python -m open_rarity.resolver.testset_resolver \
-        external --trait_sniper --rarity_sniper`
-    """
-    args = parser.parse_args()
-    logger = logging.getLogger("open_rarity_logger")
-    logger.setLevel(logging.DEBUG)
-
-    fh = logging.FileHandler(strftime("testsetresolverlog_%H_%M_%m_%d_%Y.log"))
-    fh.setLevel(logging.DEBUG)
-
-    logger.addHandler(fh)
-    resolve_remote_rarity = args.resolve_external_rarity == "external"
-
-    external_resolvers = []
-    if args.fetch_trait_sniper:
-        external_resolvers.append(RankProvider.TRAITS_SNIPER)
-        if os.environ.get("TRAIT_SNIPER_API_KEY") is None:
-            raise ValueError(
-                "TRAIT_SNIPER_API_KEY not set. Required to fetch Traits Sniper data"
-            )
-    if args.fetch_rarity_sniffer:
-        external_resolvers.append(RankProvider.RARITY_SNIFFER)
-    if args.fetch_rarity_sniper:
-        external_resolvers.append(RankProvider.RARITY_SNIPER)
-
-    print(
-        "Welcome to OpenRarity resolver! This is a tool to view OpenRarity rankings \n"
-        "for given collection(s) and to compare them with existing ranking \n"
-        "providers. If you just want to output OpenRarity rankings, you can use "
-        "the script scripts/score_real_collections.py. \nFor full options, "
-        "run `python3 -m open_rarity.resolver.testset_resolver --help`"
-    )
-    print(f"\nExecuting args: {args}")
-    if resolve_remote_rarity:
-        print(
-            f"Fetching external ranks from: {[rp.value for rp in external_resolvers]}"
-        )
-
-    print(
-        "\nNOTE: Resolving external data can take awhile due to external API rate"
-        "\nlimits. Local caching will occur automatically so that future runs of "
-        "\nthe same collection can be efficient. Expect a 10k collection to take >5 min"
-        "\nwithout local cached data (timing based on exact external resolver(s) set). "
-        "\nWith caching, expect ~15 seconds for processing."
-    )
-
-    resolve_collection_data(
-        resolve_remote_rarity,
-        external_rank_providers=external_resolvers,
-        use_cache=args.cache_fetched_data,
-        filename=args.filename,
-    )
+# import argparse
+# import csv
+# import io
+# import json
+# import logging
+# import math
+# import pkgutil
+# from dataclasses import dataclass
+# from time import process_time, strftime
+
+# import numpy as np
+
+# from openrarity.collection.collection import Collection
+# from openrarity.token.identifier import EVMContractTokenIdentifier
+# from openrarity.token.rarity import TokenRarity
+# from openrarity.token.token import Token
+# from openrarity.providers.external_rarity_provider import (
+#     EXTERNAL_RANK_PROVIDERS,
+#     ExternalRarityProvider,
+# )
+# from openrarity.providers.collection import CollectionWithMetadata
+# from openrarity.providers.token import (
+#     RankProvider,
+#     RarityData,
+#     TokenWithRarityData,
+# )
+# from openrarity.providers.opensea import get_collection_with_metadata_from_opensea
+# from openrarity.rarity_ranker import RarityRanker
+# from openrarity.scorers.features import TokenFeatureExtractor
+# from openrarity.scorers.information_content import IC
+# from openrarity.scorers.sum_scoring_handler import SumScoringHandler
+
+# sum_handler = SumScoringHandler()
+# ic_handler = IC()
+
+# RankScore = tuple[int, float]
+# # Token ID -> Score
+# ScoredTokens = dict[int, float]
+# # Token ID -> Rank + Score
+# RankedTokens = dict[int, RankScore]
+
+# logger = logging.getLogger("open_rarity_logger")
+
+
+# parser = argparse.ArgumentParser()
+# parser.add_argument(
+#     "resolve_external_rarity",
+#     type=str,
+#     default=None,
+#     help="Specify 'external' if you want to resolve rarity from external providers",
+# )
+
+# parser.add_argument(
+#     "--cache",
+#     dest="cache_fetched_data",
+#     action=argparse.BooleanOptionalAction,
+#     default=True,
+#     help="Whether we use local data files to cache external trait + rank data",
+# )
+# parser.add_argument(
+#     "--filename",
+#     dest="filename",
+#     default="test_collections.json",
+#     help="File in /data folder containing collections to resolve.",
+# )
+
+
+# @dataclass
+# class OpenRarityScores:
+#     arithmetic_scores: RankedTokens
+#     geometric_scores: RankedTokens
+#     harmonic_scores: RankedTokens
+#     sum_scores: RankedTokens
+#     information_content_scores: RankedTokens
+
+
+# def get_tokens_with_rarity(
+#     collection_with_metadata: CollectionWithMetadata,
+#     external_rank_providers: list[RankProvider] = EXTERNAL_RANK_PROVIDERS,
+#     resolve_remote_rarity: bool = True,
+#     batch_size: int = 300,
+#     max_tokens_to_calculate: int = None,
+#     cache_external_ranks: bool = True,
+# ) -> list[TokenWithRarityData]:
+#     """Resolves assets through OpenSea API asset endpoint and turns them
+#     into token with rarity data, augmented with rankings from Gem, RaritySniper
+#     and TraitSniper.
+
+#     Parameters
+#     ----------
+#     collection : Collection
+#         collection
+#     resolve_remote_rarity : bool
+#         True if we need to resolve rarity ranks from
+#         external providers , False if not
+#     max_tokens_to_calculate (int, optional): If specified only gets ranking
+#         data of first `max_tokens`. Defaults to None.
+#     cache_external_ranks : bool
+#         If set to true, will cache external ranks into local json file and
+#         optionally use cached data if file exists. If cache file already exists,
+#         will not refetch or rewrite cache data.
+
+#     Returns
+#     -------
+#     list[TokenWithRarityData]
+#         provide list of tokens augmented with assets metadata and ranking provider
+#     """
+#     slug = collection_with_metadata.opensea_slug
+#     external_rarity_provider = ExternalRarityProvider()
+#     total_supply = min(
+#         max_tokens_to_calculate or collection_with_metadata.token_total_supply,
+#         collection_with_metadata.token_total_supply,
+#     )
+#     num_batches = math.ceil(total_supply / batch_size)
+#     tokens = collection_with_metadata.collection.tokens
+#     assert len(tokens) == collection_with_metadata.token_total_supply
+#     tokens_with_rarity: list[TokenWithRarityData] = []
+
+#     t1_start = process_time()
+
+#     for batch_id, tokens_batch in enumerate(np.array_split(tokens, num_batches)):
+#         message = (
+#             f"Starting batch {batch_id} for collection "
+#             f"{slug}: Processing {len(tokens_batch)} tokens"
+#         )
+#         logger.debug(message)
+#         print(message)
+
+#         # We will store all rarities calculated across providers in this list
+#         tokens_rarity_batch = [
+#             TokenWithRarityData(token=t, rarities=[]) for t in tokens_batch
+#         ]
+
+#         if resolve_remote_rarity:
+#             external_rarity_provider.fetch_and_update_ranks(
+#                 collection_with_metadata=collection_with_metadata,
+#                 tokens_with_rarity=tokens_rarity_batch,
+#                 rank_providers=external_rank_providers,
+#                 cache_external_ranks=cache_external_ranks,
+#             )
+#         # Add the batch of augmented tokens with rarity into return value
+#         tokens_with_rarity.extend(tokens_rarity_batch)
+
+#     # Cache the data
+#     if cache_external_ranks:
+#         for rank_provider in external_rank_providers:
+#             external_rarity_provider.write_cache_to_file(
+#                 slug=slug, rank_provider=rank_provider
+#             )
+
+#     t1_stop = process_time()
+#     logger.debug(
+#         "Elapsed time during the asset resolution in seconds {seconds}".format(
+#             seconds=t1_stop - t1_start
+#         )
+#     )
+
+#     return tokens_with_rarity
+
+
+# def resolve_collection_data(
+#     resolve_remote_rarity: bool,
+#     package_path: str = "open_rarity.data",
+#     filename: str = "test_collections.json",
+#     max_tokens_to_calculate: int = None,
+#     use_cache: bool = True,
+# ) -> None:
+#     """Resolves collection information through OpenSea API
+
+#     Parameters
+#     ----------
+#     resolve_remote_rarity : bool
+#         Set to true to resolve external rarity ranks for rank comparisons
+#     package_path : str, optional
+#         The package path for where the collection data to resolve collection data lives,
+#         by default "open_rarity.data"
+#     filename : str, optional
+#         The filename of the file holding the collection slugs to resolve,
+#         by default "test_collections.json"
+#     max_tokens_to_calculate : int, optional
+#         If specified only gets ranking data of first `max_tokens`, by default None.
+#         Note: If this is provided, we cannot calculate OpenRarity ranks since
+#         it must be calculated after calculating scoring for entire collection.
+#     use_cache: bool
+#         If set to true, will cache fetched data from external API's in order to ensure
+#         re-runs for same collections are faster. Only use if collection and token
+#         metadata is static - do not work for unrevealed/changing collections.
+
+#     Raises
+#     ------
+#     ValueError
+#         If the file containing collection slugs to resolve does not exist.
+#     """
+#     golden_collections = pkgutil.get_data(package_path, filename)
+#     if not golden_collections:
+#         raise ValueError("Can't resolve golden collections data file.")
+
+#     data = json.load(io.BytesIO(golden_collections))
+#     for collection_def in data:
+#         opensea_slug = collection_def["collection_slug"]
+#         print(f"Fetching collection and token trait data for: {opensea_slug}")
+#         # Fetch collection metadata and tokens that belong to this collection
+#         # from opensea and other external api's.
+#         collection_with_metadata = get_collection_with_metadata_from_opensea(
+#             opensea_collection_slug=opensea_slug,
+#             use_cache=use_cache,
+#         )
+#         print(f"Fetching external rarity ranks for: {opensea_slug}")
+#         tokens_with_rarity: list[TokenWithRarityData] = get_tokens_with_rarity(
+#             collection_with_metadata=collection_with_metadata,
+#             resolve_remote_rarity=resolve_remote_rarity,
+#             max_tokens_to_calculate=max_tokens_to_calculate,
+#             cache_external_ranks=use_cache,
+#         )
+#         print(f"\t=>Finished fetching external rarity ranks for: {opensea_slug}")
+
+#         collection = collection_with_metadata.collection
+
+#         if max_tokens_to_calculate is None:
+#             assert collection.token_total_supply == len(tokens_with_rarity)
+#         else:
+#             assert max_tokens_to_calculate == len(tokens_with_rarity)
+
+#         # Calculate and append open rarity scores
+#         if max_tokens_to_calculate is None:
+#             open_rarity_scores = resolve_open_rarity_score(
+#                 collection, collection.tokens
+#             )
+#             augment_with_open_rarity_scores(
+#                 tokens_with_rarity=tokens_with_rarity,
+#                 scores=open_rarity_scores,
+#             )
+
+#         serialize_to_csv(
+#             collection_with_metadata=collection_with_metadata,
+#             tokens_with_rarity=tokens_with_rarity,
+#         )
+
+
+# def augment_with_open_rarity_scores(
+#     tokens_with_rarity: list[TokenWithRarityData], scores: OpenRarityScores
+# ) -> None:
+#     """Augments tokens_with_rarity with ranks and scores computed by
+#     OpenRarity scorers'"""
+#     for token_with_rarity in tokens_with_rarity:
+#         token_id = token_with_rarity.token.token_identifier.token_id  # type: ignore
+
+#         token_with_rarity.rarities.extend(
+#             [
+#                 RarityData(
+#                     provider=RankProvider.OR_ARITHMETIC,
+#                     rank=scores.arithmetic_scores[token_id][0],
+#                     score=scores.arithmetic_scores[token_id][1],
+#                 ),
+#                 RarityData(
+#                     provider=RankProvider.OR_GEOMETRIC,
+#                     rank=scores.geometric_scores[token_id][0],
+#                     score=scores.geometric_scores[token_id][1],
+#                 ),
+#                 RarityData(
+#                     provider=RankProvider.OR_HARMONIC,
+#                     rank=scores.harmonic_scores[token_id][0],
+#                     score=scores.harmonic_scores[token_id][1],
+#                 ),
+#                 RarityData(
+#                     provider=RankProvider.OR_SUM,
+#                     rank=scores.sum_scores[token_id][0],
+#                     score=scores.sum_scores[token_id][1],
+#                 ),
+#                 RarityData(
+#                     provider=RankProvider.OR_INFORMATION_CONTENT,
+#                     rank=scores.information_content_scores[token_id][0],
+#                     score=scores.information_content_scores[token_id][1],
+#                 ),
+#             ]
+#         )
+
+
+# def extract_rank(tokens_to_score: dict[int, TokenRarity]) -> RankedTokens:
+#     """Sorts dictionary by float score and extract rank according to the score
+
+#     Parameters
+#     ----------
+#     token_id_to_scores : dict[int, TokenRarity]
+#         dictionary of token_id_to_scores with token_id to score mapping
+
+#     Returns
+#     -------
+#     dict[int, RankScore]
+#         dictionary of token to rank, score pair
+#     """
+#     ranked_tokens: list[TokenRarity] = RarityRanker.set_rarity_ranks(
+#         token_rarities=tokens_to_score.values()
+#     )
+#     return {
+#         int(token.token.token_identifier.token_id): (
+#             token.rank,
+#             token.score,
+#         )
+#         for token in ranked_tokens
+#     }
+
+
+# def resolve_open_rarity_score(
+#     collection: Collection, tokens: list[Token]
+# ) -> OpenRarityScores:
+#     """Resolve scores from all scorers with trait_normalization
+
+#     Parameters
+#     ----------
+#     collection : Collection
+#         collection is needed since the score is based on the invdividual's traits
+#         probability across the entire collection
+#     tokens: Subset of tokens belonging to Collection to resolve open rarity scores for
+
+#     """
+#     t1_start = process_time()
+
+#     # Dictionaries of token IDs to their respective TokenRarity for each strategy
+#     arthimetic_dict: dict[str, TokenRarity] = {}
+#     geometric_dict: dict[str, TokenRarity] = {}
+#     harmonic_dict: dict[str, TokenRarity] = {}
+#     sum_dict: dict[str, TokenRarity] = {}
+#     ic_dict: dict[str, TokenRarity] = {}
+
+#     logger.debug("OpenRarity scoring")
+
+#     for token in tokens:
+#         token_identifier = token.token_identifier
+#         assert isinstance(token_identifier, EVMContractTokenIdentifier)
+#         token_id = str(token_identifier.token_id)
+
+#         try:
+#             token_features = TokenFeatureExtractor.extract_unique_attribute_count(
+#                 token=token, collection=collection
+#             )
+
+#             harmonic_dict[token_id] = TokenRarity(
+#                 token=token,
+#                 token_features=token_features,
+#                 score=harmonic_handler.score_token(collection=collection, token=token),
+#             )
+#             arthimetic_dict[token_id] = TokenRarity(
+#                 token=token,
+#                 token_features=token_features,
+#                 score=arithmetic_handler.score_token(
+#                     collection=collection, token=token
+#                 ),
+#             )
+#             geometric_dict[token_id] = TokenRarity(
+#                 token=token,
+#                 token_features=token_features,
+#                 score=geometric_handler.score_token(collection=collection, token=token),
+#             )
+#             sum_dict[token_id] = TokenRarity(
+#                 token=token,
+#                 token_features=token_features,
+#                 score=sum_handler.score_token(collection=collection, token=token),
+#             )
+#             ic_dict[token_id] = TokenRarity(
+#                 token=token,
+#                 token_features=token_features,
+#                 score=ic_handler.score_token(collection=collection, token=token),
+#             )
+
+#         except Exception:
+#             logger.exception(f"Can't score token {token} with OpenRarity")
+
+#     # Calculate ranks of all assets given the scores
+#     arthimetic_ranked_tokens = extract_rank(arthimetic_dict)
+#     geometric_ranked_tokens = extract_rank(geometric_dict)
+#     harmonic_ranked_tokens = extract_rank(harmonic_dict)
+#     sum_ranked_tokens = extract_rank(sum_dict)
+#     ic_ranked_tokens = extract_rank(ic_dict)
+
+#     t1_stop = process_time()
+#     logger.debug(
+#         "OpenRarity scores resolution in seconds {seconds}".format(
+#             seconds=t1_stop - t1_start
+#         )
+#     )
+
+#     return OpenRarityScores(
+#         arithmetic_scores=arthimetic_ranked_tokens,
+#         geometric_scores=geometric_ranked_tokens,
+#         harmonic_scores=harmonic_ranked_tokens,
+#         sum_scores=sum_ranked_tokens,
+#         information_content_scores=ic_ranked_tokens,
+#     )
+
+
+# def _get_provider_rank(
+#     provider: RankProvider, token_with_rarity: TokenWithRarityData
+# ) -> int | None:
+#     """Get rank for the particular provider
+
+#     Parameters
+#     ----------
+#     provider : RankProvider
+#         rank provider
+#     token : Token
+#         token
+#     """
+#     rarities = token_with_rarity.rarities
+#     rarity_datas = list(filter(lambda rarity: rarity.provider == provider, rarities))
+#     return rarity_datas[0].rank if len(rarity_datas) > 0 else None
+
+
+# def _rank_diff(rank1: int | None, rank2: int | None) -> int | None:
+#     """Function that computes the rank difference
+
+#     Parameters
+#     ----------
+#     rank1 : int | None
+#         rank of the asset
+#     rank2 : int | None
+#         rank of the asset
+
+#     Returns
+#     -------
+#     int | None
+#         absolute difference of ranks for the specific asset
+#     """
+#     if not rank1 or not rank2:
+#         return None
+
+#     return abs(rank1 - rank2)
+
+
+# def serialize_to_csv(
+#     collection_with_metadata: CollectionWithMetadata,
+#     tokens_with_rarity: list[TokenWithRarityData],
+# ) -> None:
+#     """Serialize collection and ranking data to CSV
+
+#     Parameters
+#     ----------
+#     collection : Collection
+#         collection
+#     """
+#     slug = collection_with_metadata.opensea_slug
+#     testset = open(f"testset_{slug}.csv", "w")
+#     headers = [
+#         "slug",
+#         "token_id",
+#         "traits_sniper",
+#         "rarity_sniffer",
+#         "rarity_sniper",
+#         "arithmetic",
+#         "geometric",
+#         "harmonic",
+#         "sum",
+#         "information_content",
+#         "traits_sniper_rarity_sniffer_diff",
+#         "traits_sniper_rarity_sniper_diff",
+#         "traits_sniper_arithm_diff",
+#         "traits_sniper_geom_diff",
+#         "traits_sniper_harmo_diff",
+#         "traits_sniper_sum_diff",
+#         "traits_sniper_ic_diff",
+#         "rarity_sniffer_rarity_sniper_diff",
+#         "rarity_sniffer_arithm_diff",
+#         "rarity_sniffer_geom_diff",
+#         "rarity_sniffer_harmo_diff",
+#         "rarity_sniffer_sum_diff",
+#         "rarity_sniffer_ic_diff",
+#         "rarity_sniper_arithm_diff",
+#         "rarity_sniper_geom_diff",
+#         "rarity_sniper_harmo_diff",
+#         "rarity_sniper_sum_diff",
+#         "rarity_sniper_ic_diff",
+#     ]
+
+#     writer = csv.writer(testset)
+#     writer.writerow(headers)
+
+#     for token_with_rarity in tokens_with_rarity:
+#         traits_sniper_rank = _get_provider_rank(
+#             RankProvider.TRAITS_SNIPER, token_with_rarity
+#         )
+#         rarity_sniffer_rank = _get_provider_rank(
+#             RankProvider.RARITY_SNIFFER, token_with_rarity
+#         )
+#         rarity_sniper_rank = _get_provider_rank(
+#             RankProvider.RARITY_SNIPER, token_with_rarity
+#         )
+#         or_arithmetic_rank = _get_provider_rank(
+#             RankProvider.OR_ARITHMETIC, token_with_rarity
+#         )
+#         or_geometric_rank = _get_provider_rank(
+#             RankProvider.OR_GEOMETRIC, token_with_rarity
+#         )
+#         or_harmonic_rank = _get_provider_rank(
+#             RankProvider.OR_HARMONIC, token_with_rarity
+#         )
+#         or_sum_rank = _get_provider_rank(RankProvider.OR_SUM, token_with_rarity)
+#         or_ic_rank = _get_provider_rank(
+#             RankProvider.OR_INFORMATION_CONTENT, token_with_rarity
+#         )
+#         row = [
+#             slug,
+#             token_with_rarity.token.token_identifier.token_id,  # type: ignore
+#             traits_sniper_rank,
+#             rarity_sniffer_rank,
+#             rarity_sniper_rank,
+#             or_arithmetic_rank,
+#             or_geometric_rank,
+#             or_harmonic_rank,
+#             or_sum_rank,
+#             or_ic_rank,
+#             _rank_diff(traits_sniper_rank, rarity_sniffer_rank),
+#             _rank_diff(traits_sniper_rank, rarity_sniper_rank),
+#             _rank_diff(traits_sniper_rank, or_arithmetic_rank),
+#             _rank_diff(traits_sniper_rank, or_geometric_rank),
+#             _rank_diff(traits_sniper_rank, or_harmonic_rank),
+#             _rank_diff(traits_sniper_rank, or_sum_rank),
+#             _rank_diff(traits_sniper_rank, or_ic_rank),
+#             _rank_diff(rarity_sniffer_rank, rarity_sniper_rank),
+#             _rank_diff(rarity_sniffer_rank, or_arithmetic_rank),
+#             _rank_diff(rarity_sniffer_rank, or_geometric_rank),
+#             _rank_diff(rarity_sniffer_rank, or_harmonic_rank),
+#             _rank_diff(rarity_sniffer_rank, or_sum_rank),
+#             _rank_diff(rarity_sniffer_rank, or_ic_rank),
+#             _rank_diff(rarity_sniper_rank, or_arithmetic_rank),
+#             _rank_diff(rarity_sniper_rank, or_geometric_rank),
+#             _rank_diff(rarity_sniper_rank, or_harmonic_rank),
+#             _rank_diff(rarity_sniper_rank, or_sum_rank),
+#             _rank_diff(rarity_sniper_rank, or_ic_rank),
+#         ]
+#         writer.writerow(row)
+
+
+# if __name__ == "__main__":
+#     """Script to resolve external datasets and compute rarity scores
+#     on test collections. Data resolved from opensea api
+
+#     command to run:
+#     python -m  openrarity.resolver.testset_resolver external
+#     """
+#     args = parser.parse_args()
+#     logger = logging.getLogger("open_rarity_logger")
+#     logger.setLevel(logging.DEBUG)
+
+#     fh = logging.FileHandler(strftime("testsetresolverlog_%H_%M_%m_%d_%Y.log"))
+#     fh.setLevel(logging.DEBUG)
+
+#     logger.addHandler(fh)
+#     resolve_remote_rarity = args.resolve_external_rarity
+
+#     print(f"Executing main: with {args}")
+#     resolve_collection_data(
+#         resolve_remote_rarity,
+#         use_cache=args.cache_fetched_data,
+#         filename=args.filename,
+#     )
```

### Comparing `open_rarity-0.7.2/pyproject.toml` & `open-rarity-1.0.0a1/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,59 +1,66 @@
 [tool.poetry]
-authors = ["Dan Meshkov <daniil.meshkov@opensea.io>", "Vicky Gong <vicky.gong@opensea.io>"]
+authors = ["Dan Meshkov <daniil.meshkov@opensea.io>", "Vicky Gong <vicky.gong@opensea.io>", "Taylor Beever <taylor@quicknode.com>"]
 description = "Open-Rarity library is an open standard that provides an easy, explanable and reproducible computation for NFT rarity"
 license = "Apache-2.0"
 name = "open-rarity"
-version = "0.7.2"
+packages = [
+  {include = "openrarity"},
+  {include = "openrarity/py.typed"},
+]
+version = "1.0.0a1"
 
 readme = "README.md"
 
 classifiers = [
   "Programming Language :: Python :: 3",
   "Programming Language :: Python",
   "Intended Audience :: Developers",
   "License :: OSI Approved :: Apache Software License",
   "Natural Language :: English",
   "Typing :: Typed",
   "Topic :: Software Development :: Libraries",
   "Development Status :: 4 - Beta",
   "Programming Language :: Python :: 3.10",
-  "Programming Language :: Python :: 3.11",
 ]
+[tool.poetry.scripts]
+openrarity = "openrarity.cli.main:app"
 
 [tool.poetry.dependencies]
-numpy = "^1.23.1"
-pandas = "^1.4.3"
-pydantic = ">=1.9.1,<2.1"
+aiolimiter = "^1.0.0"
+httpx = "^0.23.0"
+numpy = "^1.23.4"
+pysatchel = "^0.3.1"
 python = ">=3.10,<3.12"
-requests = "^2.28.1"
-scipy = "^1.9.0"
+tabulate = "^0.9.0"
+tenacity = "^8.1.0"
+tqdm = "^4.64.1"
+typer = "^0.6.1"
 
-[tool.poetry.group.dev.dependencies]
-black = "^23.7.0"
+[tool.poetry.dev-dependencies]
+black = "^22.6.0"
 flake8 = "^5.0.2"
 flake8-bugbear = "^22.7.1"
 isort = "^5.10.1"
-mypy = "^0.982"
+jupyterlab = "^3.4.8"
+matplotlib = "^3.6.1"
+mypy = "^0.971"
+pandas = "^1.5.1"
 pep8-naming = "^0.13.1"
 pre-commit = "^2.19.0"
+pyarrow = "^10.0.0"
 pytest = "^7.1"
 pytest-cov = "^3.0"
-pytest-mock = "^3.10.0"
 types-requests = "^2.28.6"
 
 [tool.black]
 line-length = 88
 
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core>=1.0.0"]
 
 [tool.isort]
 include_trailing_comma = true
-known_first_party = "open_rarity"
+known_first_party = "openrarity"
 multi_line_output = 3
 profile = "black"
-
-[[tool.mypy.overrides]]
-module = ["scipy", "scipy.stats"]
-ignore_missing_imports = true
```

### Comparing `open_rarity-0.7.2/PKG-INFO` & `open-rarity-1.0.0a1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 Metadata-Version: 2.1
 Name: open-rarity
-Version: 0.7.2
+Version: 1.0.0a1
 Summary: Open-Rarity library is an open standard that provides an easy, explanable and reproducible computation for NFT rarity
 License: Apache-2.0
 Author: Dan Meshkov
 Author-email: daniil.meshkov@opensea.io
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Typing :: Typed
-Requires-Dist: numpy (>=1.23.1,<2.0.0)
-Requires-Dist: pandas (>=1.4.3,<2.0.0)
-Requires-Dist: pydantic (>=1.9.1,<2.1)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
-Requires-Dist: scipy (>=1.9.0,<2.0.0)
+Requires-Dist: aiolimiter (>=1.0.0,<2.0.0)
+Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: numpy (>=1.23.4,<2.0.0)
+Requires-Dist: pysatchel (>=0.3.1,<0.4.0)
+Requires-Dist: tabulate (>=0.9.0,<0.10.0)
+Requires-Dist: tenacity (>=8.1.0,<9.0.0)
+Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Requires-Dist: typer (>=0.6.1,<0.7.0)
 Description-Content-Type: text/markdown
 
 ![OpenRarity](img/OR_Github_banner.jpg)
 
 [![Version][version-badge]][version-link]
 [![Test CI][ci-badge]][ci-link]
 [![License][license-badge]][license-link]
@@ -34,46 +38,70 @@
 
 We’re excited to announce OpenRarity, a new rarity protocol we’re building for the NFT community. Our objective is to provide a transparent rarity calculation that is entirely open-source, objective, and reproducible.
 
 With the explosion of new collections, marketplaces and tooling in the NFT ecosystem, we realized that rarity ranks often differed across platforms which could lead to confusion for buyers, sellers and creators. We believe it’s important to find a way to provide a unified and consistent set of rarity rankings across all platforms to help build more trust and transparency in the industry.
 
 We are releasing the OpenRarity library in a Beta preview to crowdsource feedback from the community and incorporate it into the library evolution.
 
-See the full announcement in the [blog post](https://mirror.xyz/openrarity.eth/-R8ZA5KCMgqtsueySlruAhB77YBX6fSnS_dT-8clZPQ).
+See the full announcement in the [blog post](https://mirror.xyz/openrarity.eth/LUoJnybWuNYedIQHD6RRdX1SS9MiowdI6a69X-lefGM).
 
-# Developer documentation
+## CLI Usage
 
-Read [developer documentation](https://openrarity.gitbook.io/developers/) on how to integrate with OpenRarity.
 
-# Setup and run tests locally
+If you already have a json file containing the metadata for the tokens you want to rank you can run the following which will print ranks to stdout.
 
 ```
-poetry install # install dependencies locally
-poetry run pytest # run tests
+❯ openrarity rank data/boredapeyachtclub/tokens.json | head -n 10
+  token_id    unique_traits       ic    rank
+----------  ---------------  -------  ------
+      7495                0  42.0592       1
+      4873                0  40.4554       2
+      8854                0  40.2091       3
+       446                0  40.017        4
+        73                0  39.6501       5
+      8135                0  39.5842       6
+      8976                0  39.5072       7
+      4980                0  39.4849       8
 ```
 
-Some tests are skipped by default due to it being more integration/slow tests.
-To run resolver tests:
+Likewise you can write to a json file
 ```
-poetry run pytest -k test_testset_resolver --run-resolvers
+❯ openrarity rank data/boredapeyachtclub/tokens.json -o boredapeyachtclub_ranks.json
 ```
 
-# Library usage
-You can install open rarity as a [python package](https://pypi.org/project/open-rarity/) to use OpenRarity in your project:
+
+If you don't have metadata available you can fetch it from OpenSea first
 ```
-pip install open-rarity
+❯ openrarity opensea fetch-assets --slug boredapeyachtclub --start-token-id 0 --end-token-id 9999 --rank | head -n 10
+100%|████████████████████████████████████████| 334/334 [01:40<00:00,  3.33it/s]
+  token_id    unique_traits       ic    rank
+----------  ---------------  -------  ------
+      7495                0  42.0592       1
+      4873                0  40.4554       2
+      8854                0  40.2091       3
+       446                0  40.017        4
+        73                0  39.6501       5
+      8135                0  39.5842       6
+      8976                0  39.5072       7
+      4980                0  39.4849       8
 ```
-Please refer to the [scripts/](/scripts/) folder for an example of how to use the library.
 
-If you have downloaded the repo, you can use OpenRarity shell tool to generate json or csv outputs of OpenRarity scoring and ranks for any collections:
+# Developer documentation
+
+Read [developer documentation](https://openrarity.gitbook.io/developers/) on how to integrate with OpenRarity.
+
+# Setup and run tests locally
+
 ```
-python -m scripts.score_real_collections boredapeyachtclub proof-moonbirds
+poetry install # install dependencies locally
+poetry run pytest # run tests
 ```
-Read [developer documentation](https://openrarity.gitbook.io/developers/) for advanced library usage
 
+# Library usage
+Read [developer documentation](https://openrarity.gitbook.io/developers/) for advanced library usage
 
 
 # Contributions guide and governance
 
 OpenRarity is a community effort to improve rarity computation for NFTs (Non-Fungible Tokens). The core collaboration group consists of four primary contributors: [Curio](https://curio.tools), [icy.tools](https://icy.tools), [OpenSea](https://opensea.io) and [Proof](https://www.proof.xyz/)
 
 OpenRarity is an open-source project and all contributions are welcome. Consider following steps when you request/propose contribution:
@@ -91,15 +119,14 @@
 
 # Project Setup and Core technologies
 
 We used the following core technologies in OpenRarity:
 
 - Python ≥ 3.10.x
 - Poetry for dependency management
-- Numpy ≥1.23.1
 - PyTest for unit tests
 
 # License
 
 Apache 2.0 , OpenSea, ICY, Curio, PROOF
```

